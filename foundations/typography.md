# Typography

Keep type simple, systematic and hierarchical.

## When to use

- Choosing typefaces or weights for a design.
- Defining a type scale or text styles before designing screens.
- A screen has many font sizes/styles and feels inconsistent.
- Deciding how headings, labels, body copy and links should differ.

Font choices by vibe, and the AI-looking fonts to skip, are in `font-picks`. Button label sizes are in `buttons-and-ctas`. Placeholder vs input text color is in `forms-and-inputs`. Contrast ratios are in `color-system`.

## 1. Few typefaces, few weights

- Use one or two typefaces. Do not use every font available.
- Vary weight and size within a family instead of adding families.
- Use weight variations sparingly. Too many styles feel inconsistent and messy.
- Example hierarchy in a single family: small colored all-caps eyebrow, a heavy-weight headline, medium-weight body.

## 2. Simple, legible type for functional text

- Keep complicated or decorative type for large headlines only.
- Use simple, legible type for paragraphs, labels, buttons and everything else. Do not set body text, labels or buttons in a decorative serif and mix italic styles into UI text.

## 3. Type scale

- Define the scale before designing. Pick a base size and a ratio.
- Example from the sources: base 14px with a 1.2 ratio, six steps up and two steps down gives roughly 10, 12, 14, 17, 20, 24, 29, 35, 42px.
- A plugin such as Typescales can generate a scale in Figma.

## 4. Few font sizes, reused consistently

- Reuse the same few sizes across components. Inconsistent sizes (for example 20 / 16 / 14 / 18 on one login card) look messy; consolidate to 20 for title and button, 16 for subtitle and inputs.

## 5. Text hierarchy

Users should instantly know what to read first:
1. Heading - largest, boldest.
2. Subheading.
3. Body copy - smallest.
4. Action - colored, often an underlined link with an arrow.

Make the first thing obvious.

## Checklist

- [ ] No more than two typefaces
- [ ] Type scale defined and used everywhere
- [ ] Same number of font sizes on every similar component
- [ ] Decorative type confined to large headlines
- [ ] Clear heading / subheading / body / action levels
