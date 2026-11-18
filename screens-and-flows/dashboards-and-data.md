# Dashboards and Data Visualisation

A dashboard gives a visual snapshot of key information so users can decide quickly.

## When to use

- Designing a dashboard, analytics screen or admin panel.
- Laying out KPI cards and widgets.
- Choosing a chart type for a dataset.

Sidebar spacing is in `spacing-grid-alignment`; navigation behaviour in `navigation`; restraint and hierarchy in `visual-hierarchy-and-clean-ui`.

## 1. Purpose

Show a visual snapshot of the important information and key performance indicators to enable quick decisions and understanding. If a widget does not serve that, remove it.

## 2. Common structure

There is no strict rule, but patterns repeat:
1. **Main navigation** - usually a left sidebar: logo, grouped items with icons, active state, optional CTA or promo card at the bottom.
2. **Header panel** - breadcrumbs for hierarchy levels, a primary action button, profile menu and notifications.
3. **Grid of content widgets** - progress rings, statistic lists, tables, cards.

## 3. Grid

Think in boxes that reflect the screen width. Four common arrangements:
- A: four small KPI tiles on top, two large widgets below.
- B: one large widget, two small tiles and one tall widget.
- C: three on top; a stack of small ones on the left, one large on the right.
- D: a 2x2 block of small tiles, a tall widget on the right and a wide one at the bottom.

## 4. Widget anatomy

- Heading with an icon at the top-left.
- Filter or customization (dropdown) at the top-right.
- A link or arrow button to the full data view at the top-right.
- Content = a simplified summary of a more complex feature (for example a watchlist with price, a green/red change and a sparkline).

## 5. Scanning (F-pattern)

People scan in an F shape: along the top, then a shorter pass, then down the left edge. Put the most important information along the top and left.

## 6. Pick the chart by purpose

| Purpose | Chart options |
|---|---|
| Relationship | Scatter, bubble, network diagram |
| Comparison | Column, bar, circular area, line |
| Composition | Pie, treemap, heat map, stacked column, waterfall |
| Distribution | Scatter, histogram, bell curve |

Include a legend with values when using radial/composition charts (for example sleep: Deep 45%, Light 32%, Awake 28%, Quality 87%).

## Checklist

- [ ] Every widget earns its place; focal widget is the largest
- [ ] Structure: sidebar, header, grid
- [ ] Widgets follow one anatomy
- [ ] Key info top/left
- [ ] Chart type matches the question being asked
