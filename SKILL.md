---
name: ui-ux-tips
description: UI/UX design rules and procedures. Use when designing, building, reviewing or polishing any interface, screen, component, animation or flow, when a UI looks AI-generated or flat, or when asked for UI/UX best practices. Covers UX laws, layout, color, type and fonts, forms, auth, states, navigation, mobile, motion, plus unslop, polish and award-level procedures.
---

# UI/UX Tips (master index)

One entry point for everything UI/UX. Do not read it all. Pick the guides that match the task, read only those files, and apply their rules.

Paths below are relative to this folder (`~/.claude/skills/ui-ux-tips/`).

## How to use

1. Identify what is being designed or reviewed (a button, a form, a whole screen, a flow, an animation).
2. Look up the matching guide(s) in the tables below and read them.
3. For any full-screen design or review, also read `principles/visual-hierarchy-and-clean-ui.md` and `principles/spacing-grid-alignment.md`, and finish with `cross-cutting/design-review-checklist.md`.
4. Pick a depth with the procedures table: quick rules (guides) for ordinary work; a `procedures/` workflow when the user wants unslop, polish, motion, or award-level craft.
5. Inside the guides, backtick names such as `color-system` refer to the file with that name in this folder tree.
6. If the user names a guide or procedure ("use the buttons guide", "unslop this"), read that one directly.

## Procedures - `procedures/` (full workflows, read the PROCEDURE.md inside)

These are complete workflows (credited in README.md) bundled here. Their entry file is named `PROCEDURE.md`, not `SKILL.md`, so installers register only this skill. Read them from this folder when a task matches.

| Procedure | Read when |
|---|---|
| `procedures/unslop/PROCEDURE.md` | A screen looks AI-generated, vibe-coded, generic or templated. Audit the tells, write a direction, subtract, fix spacing/color/icons/copy/type/layout/details, give it one real moment. References: `signs.md`, `tokens.md`, `visuals.md`, `effects.md`. CC BY 4.0, credit kept in the file. |
| `procedures/polish/PROCEDURE.md` | A screen works but feels off or unfinished; hover/press/focus states, layout shift, hit areas, easing, springs, frame-by-frame motion checks, sound and haptics. If it still looks AI-made, run unslop first. |
| `procedures/ux-animation/PROCEDURE.md` | Building or reviewing how an interface moves and responds: the 20 principles of UX and animation, Emil Kowalski's rules, timing/curve tables, optimistic UI, hit areas, forms, onboarding. References: `recipes.md` (modals, drawers, popovers, toasts, icon swaps...), `techniques.md` (curves, springs, arcs, storyboards...). |
| `procedures/unreasonable-craft/PROCEDURE.md` | **Opt-in only: use when the user explicitly asks for award-level, Awwwards or Apple Design Award quality, "wow" or "stunning"; never for ordinary UI work.** The user wants award-level design (Awwwards Site of the Day, Apple Design Award), "wow", "stunning", "can't look AI-made". Heavy: explore 3+ directions, generate assets, verify frame by frame, one critique round. References: `assets.md`, `verification.md`, `critique.md`; scripts in `scripts/` (Node 18+, ffmpeg, Chrome; run `npm install` in `scripts/` first; not executed or installed yet). |

Inside those files, names like `charles-unslop` or `charles-polish`, and mentions of `SKILL.md`, mean the matching folder or its `PROCEDURE.md` here (`procedures/unslop`, `procedures/polish`). Their relative `references/` links work as-is.

Suggested order for a serious design job: `procedures/unslop` (direction and subtraction) then `procedures/ux-animation` (motion and flow) then `procedures/polish` (details and frame checks), with `procedures/unreasonable-craft` as the top-level bar when the user asks for award quality.

Note: `procedures/unreasonable-craft` mentions companion skills (`interface-craft`, `apple-design`, `animate`, `emil-design-eng`). They are not part of this bundle. Skip them if not installed; the principles in `procedures/ux-animation` and `procedures/polish` cover the same ground.

## Principles - `principles/`

| File | Read when |
|---|---|
| `ux-laws.md` | Explaining why a UI feels confusing, slow or cluttered; deciding how many options or steps to show; where key actions go (Jakob, Hick, Fitts, Miller, Proximity, Von Restorff, Serial Position, Tesler, Doherty, Peak-End). |
| `design-principles-cheatsheet.md` | Short definitions to name the principle behind a choice: Disney's 12 animation principles, Fitts/Hick/Miller/Doherty/Postel/Jakob, frequency of use, origin-aware, layout stability, labor illusion, brushing and linking, film grain, and the 8 password-flow principles (reward early punish late, closure, continuity...). |
| `visual-hierarchy-and-clean-ui.md` | A screen looks messy or flat; deciding what draws the eye first; composition, whitespace, Z/F-patterns, borders vs shadows, decoration. |
| `spacing-grid-alignment.md` | Choosing padding, margins and gaps; the 8px system; grids; alignment; nested corner radius. |

## Foundations - `foundations/`

| File | Read when |
|---|---|
| `color-system.md` | Choosing or auditing colors; palette generation in HSL; semantic, status and feedback colors; contrast. |
| `dark-mode.md` | Adding or converting to a dark theme; dark backgrounds, elevation, saturation, shadows. |
| `typography.md` | Choosing type scale, text sizes, weights, text hierarchy. |
| `font-picks.md` | Choosing a typeface by vibe (Swiss, friendly, personality, mono) and avoiding AI-looking fonts (Geist, Space Grotesk, Bricolage Grotesque, Instrument Sans, JetBrains Mono, Space Mono). |
| `font-sources.md` | You picked a font and need its licence, official page, download link or install command; also `font-sources.css`, a ready file that loads every tested font. |
| `backgrounds-and-textures.md` | A design feels flat; 22 background treatments (felt, fluted glass, halftone, grain, ASCII...), film grain against banding, rules for using texture. |
| `icons.md` | Icon sets, consistency, optical sizing, icon plus label. |

## Components - `components/`

| File | Read when |
|---|---|
| `buttons-and-ctas.md` | Any button or call to action: size, padding, hierarchy, states, labels, destructive actions, placement. |
| `forms-and-inputs.md` | Any form or input: labels, placeholders, grouping, validation, masks, multi-step progress, autocomplete. |
| `auth-screens.md` | Login, sign-up, forgot password, social login, password creation and its UX principles. |
| `selection-controls.md` | Checkbox, radio, dropdown, chips, toggle, slider; making selection state clear. |
| `feedback-states-and-dialogs.md` | Empty, error, loading and success states; toasts; tooltips; confirmation dialogs; popups. |
| `navigation.md` | Tab bars, sidebars, hamburger menus, pagination, active states. |
| `cards-and-imagery.md` | Content/product cards, photos and illustrations, text over images, linear blur, Read more. |
| `pricing-cards.md` | Pricing pages and plan cards. |

## Screens and flows - `screens-and-flows/`

| File | Read when |
|---|---|
| `dashboards-and-data.md` | Dashboards and admin home screens: start from the job, one main block, stat figures without icons, chart choice. |
| `settings-and-profile.md` | Settings, account and profile screens, account deletion. |
| `onboarding-flows.md` | Welcome/first-run flows, preference questions, reminders, free-trial explainers. |
| `mobile-ui-and-touch.md` | Phone layouts, touch targets, thumb zone, mobile spacing. |

## Examples - `examples/`

| File | Read when |
|---|---|
| `login-page-before-after.md` | You want to see how the guides combine on one screen, before and after. |

## Cross-cutting - `cross-cutting/`

| File | Read when |
|---|---|
| `component-systems.md` | An app built from shared house components (admin, back-office, CRUD, Laravel Blade, a React component library): decide font, icon policy, case, containers and density once at setup; screens look like a generic admin template. |
| `ux-writing-microcopy.md` | Any interface text: labels, errors, prompts, cancellation flows, placeholder text. |
| `design-review-checklist.md` | Before sharing or handing off a design, or when asked to review or polish one. |

## Typical combinations

- Login screen: `auth-screens`, `forms-and-inputs`, `buttons-and-ctas`
- Landing or pricing section: `pricing-cards`, `visual-hierarchy-and-clean-ui`, `buttons-and-ctas`, `typography`, `font-picks`, `backgrounds-and-textures`
- Settings page: `settings-and-profile`, `selection-controls`, `navigation`
- Admin or CRUD system with house components: `component-systems` first (at setup), then `dashboards-and-data`, `forms-and-inputs`, `navigation`, `font-picks`
- Mobile app screen: `mobile-ui-and-touch`, `navigation`, `spacing-grid-alignment`
- Design critique: `visual-hierarchy-and-clean-ui`, `spacing-grid-alignment`, `color-system`, then `design-review-checklist`
- "Make it look less AI": `procedures/unslop`, then `font-picks`, `backgrounds-and-textures`, `color-system`
- Animation or interaction work: `procedures/ux-animation`, `design-principles-cheatsheet`, then `procedures/polish` for frame checks
- Award-level site or app (only on explicit request): `procedures/unreasonable-craft`

## Resolved conflicts (apply these)

General rule: the newer, stricter procedure wins on exact numbers; the older guide keeps the "why". The user's own instruction always wins over both.

### Visual
- Shadows: prefer subtle borders; use only soft shadows when needed; one depth cue per surface.
- Dark background: default `#121212`; `#000000` only when deliberately matching iOS.
- Focus: always a visible ring, in a neutral color, at least 3:1 contrast (not a brand-colored ring).
- Neutrals and accent: tint neutrals from the product's world (blue-grey only if it fits); one accent in the chrome plus semantic colors. The 5-step accent scale is for states and tints, not extra accents.
- Backgrounds: textures and fields only on doorway screens (hero, login, empty state), with a reason. No decorative shapes or textures on working screens.
- Icons: icon-only buttons only for universal symbols. Navigation keeps icon + label. No icon on card titles, page titles, section headings, stat figures or labelled buttons unless the icon carries meaning (a warning, a status). Older guides that put an icon on widget headings are overruled (`dashboards-and-data`, `component-systems`). A project may decide to allow an icon beside a button label where it helps people find the action (Add, Export, Delete), not on every button; once decided and recorded, that is the rule for that project.
- Navigation bars: classic icon + label is the default. Floating, circle, diamond, bubble and active-text-only variants need a stated reason.
- Pricing: keep one clearly recommended card, size cards by content, and show a "Most popular" badge only if it is true. Promote annual billing visually, but the user selects the toggle themselves; never pre-select anything that costs money.

- Containers: a card only where a group needs a boundary; never a card inside a card; page titles and context lines are not in cards.
- Fonts: every project picks and installs a real font; the system font only by the user's decision (`font-picks`).

### Type and copy
- Font choice: `font-picks` wins over the "Type families" table in `procedures/unslop/references/tokens.md`. Skip the fonts font-picks lists as AI-looking (Geist, Space Grotesk, Instrument Sans, Bricolage Grotesque, JetBrains Mono, Space Mono) even where tokens.md suggests them; take a free stand-in from `font-sources`.
- Font weight: older guides suggest a heavy headline; use 400-500 (600 for rare emphasis) and build hierarchy from size and color.
- Case: sentence case for all interface text (titles, labels, buttons, menus, dialog titles, role names). Uppercase eyebrows only when the real object is uppercase. Data the business stores uppercase is shown as data in tables and fields; statuses go through a label map, never raw (`component-systems`).
- Type sizes: define a full scale if needed, but use at most 5 sizes on any one screen. Form inputs are 16px; body 14-16px.
- Tone: no exclamation marks and no greeting-style hero headlines ("Welcome back!"). Friendly, specific body copy is fine. Say the plain thing; playful only when the brand voice already exists.
- Success feedback: a check or short plain message ("Saved"), not "Looks good!" or "Saved successfully!".
- Empty states: keep headline and CTA. Add sub-copy only if it adds information; use an illustration only if it was drawn for this product.
- Placeholder text: at least 4.5:1 contrast but visibly lighter than the entered value.

### Behaviour and motion
- Touch targets: at least 44px for anything tapped; 40px only for mouse-only desktop.
- Loading: the pressed state shows on the same frame. Show a spinner or "Saving..." only after about 300ms and hold it at least 500ms. Use a skeleton only after about 1s and only where results appear, sized to the content; otherwise the trigger's pending state is enough.
- Validation timing: positive progress shows immediately; error messages wait until the field is finished (blur or submit). Once an error shows, re-check on every keystroke so it clears. Exception: a clearly bad value (a known common password such as `Password1!`) may be flagged immediately.
- Destructive actions: reversible actions get an Undo toast (5s or more) instead of a confirmation. Irreversible actions get a confirmation whose button names the verb and object ("Delete 3 files"); Cancel has default focus. A project may choose to confirm every delete and add an Undo toast (8s) afterwards for records that matter (referenced by others, costly to recreate, bulk deletes); once decided and recorded, that is the rule for that project.
- Progress: one progress indicator per flow (a stepper or a bar, not both).
- Motion frequency: anything fired many times a session or from the keyboard gets no animation; keep press/hover feedback at 100-150ms regardless.
- Tooltip duration: 125ms (other popovers 150-250ms).
