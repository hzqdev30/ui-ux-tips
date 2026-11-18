# Color System

Color communicates importance and state, not decoration. Every color needs a job.

## When to use

- Choosing a palette or adding a color to a design.
- Generating tints, shades and neutrals from one base color.
- Deciding the color of buttons, status badges, alerts, selected items.
- Auditing a screen where "color is everywhere".

Dark mode: see `dark-mode`. Button state structure: see `buttons-and-ctas`. Text contrast on images: see `cards-and-imagery`.

## 1. The four roles

| Role | Purpose | Notes |
|---|---|---|
| Primary | Brand color, most prominent | One or two colors is ideal |
| Accent | Actions, highlights | Derive from primary with color-wheel relationships: analogous, monochromatic, complementary, split complementary, triadic |
| Semantic | System meaning | Red = error/danger; green = success/safety; yellow/orange = warning/caution; blue = information |
| Neutral | Structure | Text, borders, icons, backgrounds, sections |

A simple system: 1 primary brand tone, a 5-step accent scale (light to dark), 5 neutrals (white to near-black), and 4 status colors (red, green, orange, yellow).

## 2. Functional palette

- Feedback color is for error/status only. Do not use red for a primary button or a close icon.
- Primary color marks the action. Neutrals build structure (borders, dividers, backgrounds).
- Chaotic example: red Sign Up button, red close icon, black social buttons, heavy black field borders. Functional example: primary-colored Sign Up, neutral close icon, outlined social buttons, red only on the invalid field and its message.
- Primary actions use the highest contrast, not a semantic color.

## 3. Proportion and restraint

- Limit the palette: about three core colors. Use the 60-30-10 rule: 60% neutral (often white), 30% dark secondary, 10% accent/primary.
- Start in black and white, craft the layout, then highlight deliberately.
- Structural color (neutral card tints) is separate from semantic color (a red notification dot). Do not tint every card a different color.
- Use primary mainly on the most important elements.
- Use color with purpose and never as the only signal: pair it with an icon or text (accessibility).
- Limit selection colors to two: one color means "selected". Inactive items are grey, the active item is the accent color.
- Use color to classify (status pills such as shortlisted / rejected / in process) instead of leaving everything plain grey text.

## 4. Neutrals

- Instead of pure grey, use a scale of neutral blue (a desaturated blue-grey) for a modern, clean look.
- Keep a defined set of grays and use tokens. Five almost-identical grays (#6E6E6E, #707070, #737373...) signal a detached style; use the token.

## 5. Generate a palette in HSL

Starting point: pick a base color (example H 223, S 93, L 59).
1. **Tints**: add +10 lightness repeatedly (69, 79, 89), cap the lightest near 95. Keep H and S.
2. **Shades**: subtract 10 lightness (49, 39, 29, 19).
3. **Black and white**: set lightness to about 8 and 98 and reduce saturation (for example S 20) while keeping the base hue. This gives a tinted near-black and near-white.
4. **Grayscale**: build the same way, tinted with the base hue, between the near-black and near-white.
5. **Pro tip**: increase saturation as you move away from the base color so tints and shades do not look washed out (for example S 50 base, tints up to S 70, darkest shade up to S 90).

## 6. Color in interactive states

- Hover: slightly lighter or tinted than default. Pressed: back to the base or a press indication. Focused: a visible ring or outline. Loading: same fill with a loading label. Disabled: very light grey fill and grey text.
- Hierarchy through color: primary (solid, highest contrast), secondary (light tint or outline), tertiary (text only), each with the same state logic.

## 7. Color in feedback

Banners and alerts use a tinted background, matching border, text, icon and close control:
- Info - blue with an "i/!" circle
- Warning - orange/amber with a triangle
- Success - green with a check
- Error - red with a no-entry or cross icon

## 8. Contrast

- Text on a fill needs 4.5:1 contrast (3:1 is the floor for large, bold text). A pale fill with white text at 1.3:1 is a bug, not a style.

## Examples of palette pairings seen in the sources

- Dark green primary with orange CTA and peach tint.
- Navy primary with orange-red accent and one solid plus one outline button.
- Lime primary with violet accent on a dark slate neutral.
- Green primary with violet CTA and navy headline.

## Checklist

- [ ] Each color has one role (brand, action, feedback or structure)
- [ ] Red/green/amber/blue used only for their meanings
- [ ] Palette has about three core colors
- [ ] Selected state uses one consistent color
- [ ] No meaning conveyed by color alone
- [ ] Text contrast meets 4.5:1
