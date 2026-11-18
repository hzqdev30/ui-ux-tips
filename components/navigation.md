# Navigation

Navigation should be familiar, short, and obvious about where the user is.

## When to use

- Designing a bottom tab bar, sidebar, header or menu.
- Choosing how many items navigation can hold and how to label them.
- Showing the current location (active state).
- Designing pagination for lists and tables.

Numeric sidebar spacing is in `spacing-grid-alignment`. Mobile layout margins are in `mobile-ui-and-touch`. Where profile/settings should live is in `settings-and-profile`.

## 1. General rules

- Use familiar patterns (bottom tab bar with Home / Search / Notifications / Profile). See Jakob's Law in `ux-laws`.
- Limit tabs to 3-5. A six-tab bar is too many; trim to about four.
- Keep labels short ("Home", "Search", "Save", "Profile"), never long wrapped phrases like "Explore and Search".
- Pair icons with labels and highlight the active item with a tinted background and color. This improves readability, usability and accessibility.
- Limit selection colors: inactive items grey, one accent color for the active item.

## 2. Bottom navigation variants

1. **Classic** - icon plus label; active item colored/filled.
2. **With circle CTA** - a raised circular center action button.
3. **With diamond CTA** - a raised diamond-shaped center action.
4. **Floating** - a rounded pill bar above the home indicator; active icon in a tinted circle.
5. **Active text** - only the active tab shows its label, in a tinted pill.
6. **Bubble** - the active tab lifts out with a small dot indicator.

iOS reference spec: bar content about 50px high, home-indicator safe area about 34px; five tabs on a 375px screen take 75px each; icon 24px; about 7px top padding; label 12px medium weight. Tab internals from the sources: 8px between icon and label, top padding 12 or 16px and bottom 8px (the larger top padding hides the extra space the home indicator adds under the bar).

## 3. Desktop sidebar

- Structure: logo, grouped nav items with icons and a clear active state, an optional promo/CTA card near the bottom, and a collapse control.
- Collapsed state shows icons only, with a tooltip label on hover.
- Notification dots can sit on icons. (Pixel spec: `spacing-grid-alignment`.)

## 4. Hamburger menu

- Typically top-left in the header, with an avatar or actions on the right (and optionally search).
- Seen icon styles: three equal lines, outlined square button, left-aligned short lines, lines inside a tinted circle, soft white circle button. Pick one and keep it consistent.
- A small icon in a far corner is hard to hit (Fitts's Law); for complex apps put key destinations in the tab bar instead of hiding them.

## 5. Pagination

Elements to choose from:
- Results summary ("Results 150 - 160 of 1096")
- Page-size selector ("Page items: 10")
- Previous/Next as arrows or as text buttons
- Numbered pages with the current page filled in the brand color (for example 13 14 [15] 16 17)
- First and last page with an ellipsis that opens a dropdown of the hidden pages (1 ... 14 [15] 16 ... 110)
- "Go to" input for jumping to a specific page

Variants seen: (1) page size + arrows + results + go-to; (2) Previous/Next text buttons + numbers + results + go-to; (3) arrows + numbers + results + go-to; (4) page size + arrows + first/last with ellipsis dropdown.

## Checklist

- [ ] 3-5 top-level items, short labels, icons with labels
- [ ] Active state clear; one accent color
- [ ] Standard pattern for the platform
- [ ] Tab bar respects safe areas
- [ ] Pagination shows current page and total context
