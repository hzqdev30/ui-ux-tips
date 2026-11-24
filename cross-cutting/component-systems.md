# Designing Inside a Component System (admin and CRUD apps)

Many apps are built from house components made once at the start (`<x-card>`, `<x-button>`, `<x-page-title>`, a sidebar, a table) and reused by every later feature. Here the look is decided **once**, at setup, and every screen inherits it. A choice skipped at setup shows up on every screen.

## When to use

- A project has, or is about to build, shared UI components that every module reuses (Laravel Blade components, a React component library, a design system).
- An admin, back-office or CRUD system: many list, form and detail screens, one dashboard.
- Screens come out clean but generic and identical ("looks like an admin template").

Read with `visual-hierarchy-and-clean-ui`, `spacing-grid-alignment`, `typography`, `font-picks` and `icons`. The dashboard is in `dashboards-and-data`.

## 1. Decide these once, at setup, and write them down

Record each decision where the team keeps design decisions (a UI/UX document, a design tokens file), so later features follow it instead of guessing.

| Decision | Default to start from | Why it matters |
|---|---|---|
| **Font** | A real interface font from `font-picks`, installed per `font-picks` (not the system font) | The system font is the strongest template signal |
| **Icon policy** | Icons in navigation and on icon-only buttons; elsewhere as the project's design source shows them. Record the choice with the other setup decisions | An icon on every heading and button, with no design source behind it, reads as a generic admin template |
| **Icon set** | One outline or line set at one size and stroke (16-20 px). Avoid a heavy solid set as the default | Solid filled icons everywhere read heavy and generic |
| **Case** | Sentence case for every piece of interface text: titles, labels, buttons, menu items, dialog titles, role names | ALL-CAPS chrome shouts and reads as a legacy system |
| **Stored uppercase data** | Data the business stores uppercase (names, codes, statuses) is shown as data, in tables and fields. Statuses are shown through a label map ("ACTIVE" becomes "Aktif"), never raw | Keeps the stored convention without letting it leak into the chrome |
| **Containers** | As the project's design source shows them; with none, a card only where a group needs a boundary | "Everything in a bordered card with a header strip" is the default admin layout |
| **Density** | One row height for tables, one for forms, taken from the project's design source; with none, 40-44 px. 44 px touch targets | Mixed densities look unplanned |
| **Depth** | As the project's design source shows it; with none, hairline borders or surface steps, one depth cue per surface | Shadow on every card adds noise |
| **Type scale** | At most 5 sizes, weights 400 and 500 (600 rare) | Keeps every screen consistent |

## 2. Build components that make the right thing easy

- **Make decoration optional and off by default.** An `icon` prop on a card or page title defaults to none. If the component API asks for an icon, every author will fill it.
- **Examples teach.** The first examples in the house docs are what every later screen copies. Keep them plain and take them from the project's design source.
- **Give the dashboard its own room.** The dashboard is the one screen that may break the standard card grid (`dashboards-and-data`). Do not force it into the list-screen pattern.
- **Empty and loading states are components too,** sized to their content: one line plus an action, not a tall card with a large grey icon.

## 3. Review with real content

- Seed realistic demo data before judging any screen: a busy day, long names, a cancelled item, a late payment. Screens judged empty always look unfinished, and repeated placeholder words hide the real layout.
- Look at the running screen at 360 px and 1440 px.
- Run `procedures/unslop` on the first two or three finished screens (dashboard, one list, one form). Fix what it finds **in the components**, so every later screen inherits the fix. Then run `procedures/polish` per screen.

## 4. House rules that conflict with this guide

A house style may fix things this guide argues against (a required icon prop, uppercase titles). Do not silently break the house rule. Name the conflict, recommend the guide's option, and let the user decide. Record the answer with the other setup decisions.

## Checklist

- [ ] Font, icon policy, icon set, case, containers, density, depth and type scale decided once and written down
- [ ] Component decoration (icons, header strips) is optional and off by default
- [ ] House examples are plain enough to copy
- [ ] Interface text in sentence case; stored uppercase data shown as data, statuses through a label map
- [ ] Reviewed with realistic seeded data at 360 px and 1440 px
- [ ] Fixes from unslop and polish applied in the components, not per screen
