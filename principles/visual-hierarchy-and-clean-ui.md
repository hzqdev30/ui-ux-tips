# Visual Hierarchy and Clean UI

Rules that make an interface instantly readable: the user should know where to look first, what is related, and what to do next. For spacing numbers use `spacing-grid-alignment`; for palettes use `color-system`; for type scales use `typography`.

## When to use

- A screen feels cluttered, noisy, flat, or "everything shouts".
- You must decide what the primary focus of a screen is.
- Laying out a page, hero/landing section, card or dashboard composition.
- Deciding whether to add decoration, shadows, gradients or containers.

## 1. Create a clear hierarchy

- The user should instantly know where to look first. Use size, weight and contrast to guide attention.
- Wrong: same font size everywhere, buttons that compete, all cards equally emphasised, no focal point.
- Right: one large heading creates focus; the primary CTA stands out; secondary actions stay subtle.
- Only one thing per screen gets the strongest emphasis. If everything stands out, nothing does.
- Give extra prominence to the most important element on a component (for example the price on a product card).
- Typography hierarchy: heading (largest, boldest), subheading, body (smallest), CTA/action (colored, link-like with an arrow). Make the first thing to read obvious.

## 2. Design less, communicate more

- Every element needs a purpose. Remove decorative components that do not improve usability.
- Example: one large revenue chart plus three KPI cards communicates more than ten widgets, a promo banner and a seven-icon nav.
- Reduce containers where the project's design source does not fix them: each container adds visual weight, so earn it.
- Do not go "super minimal" to the point of hiding meaning: add the detail that explains the process (label "Episode #1" instead of "#1"; show download percentage with a cancel control).

## 3. Whitespace and restraint

- Whitespace is structure, not waste. Doubling whitespace and padding can rescue a messy design.
- Whitespace improves clarity, focus and readability: give content room to breathe.
- Too much space makes elements feel disconnected; balance it with grouping.
- Design in black and white first, then add color deliberately (see `color-system`).
- Use a limited number of fonts and weights (see `typography`).

## 4. Borders, shadows and trends

- Avoid trends that reduce cleanliness: gradient CTAs, floating gimmick navigation. Stick to standard, solid patterns. Personality is fine, but less is more.

## 5. Visual principles

- **Symmetry**: balanced layouts feel stable and easier on the eye.
- **Rule of thirds**: place important content with intention (on a 3x3 grid, at the intersections).
- **Color theory**: color creates emotion, meaning and hierarchy. Use it to guide attention - for example one blue primary action and active chip with everything else neutral (palette rules: `color-system`).
- **Contrast**: important things must stand out clearly; low-contrast grey-on-grey hides the key action.
- **Consistency**: similar elements look and behave the same - same button style, icon, label casing and price format everywhere. Repetition builds trust.
- **Continuity**: the eye follows lines, curves and aligned elements; use alignment and flow to guide it (for example a connected step line).
- **Asymmetry, used intentionally**: one large tile plus smaller tiles creates hierarchy instead of equal, predictable blocks. Asymmetry creates hierarchy, not chaos.
- **Proximity**: group what belongs together (see `ux-laws`).

## 6. Reading patterns

- **Z-pattern** for simple pages and landing sections: logo top-left, navigation top-right, diagonal down to the media, finish at the CTA bottom-right. Place the image on the left and the headline plus CTA on the right so the eye path ends on the CTA.
- **F-pattern** for content-heavy screens (dashboards, lists): most important information along the top and the left edge.

## Checklist

- [ ] One obvious focal point per screen
- [ ] Primary CTA clearly stronger than secondary actions
- [ ] No decorative element without a function
- [ ] Containers kept to the minimum needed
- [ ] Borders and shadows consistent with the project's design source
- [ ] Consistent treatment of repeated elements
- [ ] Reading path ends on the main action
