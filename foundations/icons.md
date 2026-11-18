# Icons

Icons must look like they belong to one set and must be understood without guessing.

## When to use

- Designing or selecting icons for an interface.
- Mixing icons from different libraries.
- Deciding between icon-only and icon plus label.
- Reviewing an interface for icon consistency.

## Rules for a consistent set

1. **Consistent stroke weight.** Mixing stroke weights makes a set look unbalanced (too thin, too heavy, just right). Pick one.
2. **Optical size, not just canvas size.** A circle and a square on the same canvas look different in size. Circles and triangles need a slight overshoot so they look equal to squares.
3. **Consistent corner style.** Do not mix sharp and rounded corners; it makes icons feel like different sets.
4. **Do not mix filled and outlined without a rule.** It works only with a clear system, for example filled = active tab, outline = inactive. A filled "Saved" icon while inactive breaks the rule.
5. **Optical alignment.** A shape can be perfectly centered in its bounding box and still look off-center (play triangle, bell). Nudge it until it looks centered.
6. Use one consistent style across the interface: same rounding of vector shapes and same line width. A navigation bar that mixes filled, colored and differently drawn icons looks broken.

Pre-ship checklist: stroke weight, optical size, corner style, fill consistency, alignment.

## Usage rules

- Pair an icon with a short label. Icon-only buttons look clean but people guess wrong. Keep icon-only for universal symbols such as close (X) or search. If it needs a tooltip to explain it, it needs a label.
- In menus, put an icon next to the label and highlight the active option (tinted background plus color) for readability and accessibility.
- In settings lists, use icons universally associated with the action as an extra visual cue to scan faster.
- Typical icon-to-label gaps seen in the sources: 8px in tab bars and 8-12px in sidebar rows.

## Checklist

- [ ] One stroke weight and one corner style
- [ ] Filled/outline difference has a defined meaning
- [ ] Round and triangular icons optically sized
- [ ] Icons checked for visual centering
- [ ] Every non-universal icon has a label
