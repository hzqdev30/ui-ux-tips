# Spacing, Grid and Alignment

Consistent spacing and alignment matter more than extra visual effects. Fix these first.

## When to use

- Picking padding, margins, gaps or section spacing.
- Setting up a spacing scale or a layout grid.
- A layout looks "slightly off", uneven, cramped or random.
- Aligning labels, values, icons, cards, or nested rounded shapes.

Mobile-specific values are in `mobile-ui-and-touch`. Grouping logic (proximity) is in `ux-laws`.

## 1. Use a spacing system, not eyeballing

- Build spacing from multiples of 8 (with 4 as the half step). Do not eyeball every margin.
- Reference scale from the sources:

| Token | px |
|---|---|
| XXXS | 4 |
| XXS | 8 |
| XS | 12 |
| S | 16 |
| M | 24 |
| L | 32 |
| XL | 48 |
| XXL | 64 |
| XXXL | 80 |

- Wrong: uneven padding, inconsistent margins, crowded buttons, text touching the edge of a container.
- Right: equal spacing, aligned elements, breathing room, balanced layout.
- Spacing must be mathematically consistent. Random values (11px, 4px, 18px) read as noise; a steady 8px rhythm reads as order.
- Cramped layouts read as cluttered. More space improves readability, touch targets and balance (but too much disconnects elements).

## 2. Group with spacing

- Smaller gaps inside a group, larger gaps between groups. This is the main way layout communicates structure.
- Keep label-to-field and title-to-content gaps tight and constant.

## 3. Grids

- Use a grid for composition, consistency and alignment.
- Use fewer column variations. One system (for example a consistent two-column card layout) scales better than four competing layouts.
- Respect outer margins. Edge-to-edge content feels cramped; generous margins feel premium.
- In card grids use equal gaps horizontally and vertically.
- Design vertical rhythm intentionally. Erratic vertical gaps (6, 14, 6) feel anxious; a steady rhythm feels calm.

## 4. Alignment

- Align elements to shared edges. Use guides or grid lines; do not let things float.
- Labels and values should share a left edge; tooltips and axis labels align to the data point.
- Check every row and column for off-by-a-few-pixels items (for example one button 6px lower in a row of pricing cards).
- Align optically, not just mathematically. A play triangle or a bell centered by its bounding box looks off; nudge it until it looks centered. The eye judges alignment, not the grid.

## 5. Nested corner radius

- Inner radius = outer radius minus the padding between them (20px card with 12px padding gives an 8px inner radius). The same radius inside the same radius looks wrong.
- Balance radii: a pill-shaped button inside a card with a small radius clashes at the corners; increase the card radius so the curves feel concentric.

## 6. Reference spec: desktop sidebar (240px expanded, 88px collapsed)

- Side padding 16, top padding 24, logo block 32 tall.
- Nav items 40px high with about 12px between items; 8px between icon and label.
- Promo card in the sidebar about 120px tall with a 40px button; collapse control at the bottom.
- Collapsed state: icon-only items with a tooltip label on hover.

(See `navigation` for the navigation behaviour itself.)

## Checklist

- [ ] Every spacing value comes from the scale
- [ ] Gaps inside groups are smaller than gaps between groups
- [ ] Edges line up across rows and columns
- [ ] Optical centering checked on icons and symbols
- [ ] Nested radii are concentric
- [ ] Outer margins are generous and identical on both sides
