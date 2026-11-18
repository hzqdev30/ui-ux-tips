# Example: login page, before and after

Which guides fire, and what changes. Use it as a model for combining guides on one screen.

## Before (typical generated login)

- Purple-to-blue gradient background, glowing card, gradient "Welcome back!" heading, sparkle emoji
- Geist font, 800-weight heading, uppercase tracked labels
- Placeholders used as labels; red border on every empty field
- Full-width gradient "Login" button, 36px high; "Forgot password?" far from the password field
- Social buttons as grey logos, same weight as the primary button
- Spinner appears instantly on submit; password rules shown only after failure

## Which guides apply

| Problem | Guide |
|---|---|
| Looks AI-made (gradient, glow, sparkles, greeting) | `procedures/unslop/PROCEDURE.md` |
| Font choice | `foundations/font-picks.md`, `foundations/typography.md` |
| Background | `foundations/backgrounds-and-textures.md` |
| Labels, validation timing | `components/forms-and-inputs.md`, `principles/design-principles-cheatsheet.md` |
| Layout, CTA, forgot-password, social login | `components/auth-screens.md`, `components/buttons-and-ctas.md` |
| Touch size, spacing | `screens-and-flows/mobile-ui-and-touch.md`, `principles/spacing-grid-alignment.md` |
| Loading and error states | `components/feedback-states-and-dialogs.md`, `procedures/ux-animation/PROCEDURE.md` |

## After

- Flat neutral surface tinted toward the product's world; one accent for the primary button only. Film grain only if a gradient is kept.
- One interface family from `font-picks` (not on the AI-looking list); weights 400-500, sentence case.
- Real labels above fields, example placeholders. Progress shows as the person types; error text waits until the field is finished, then clears per keystroke.
- Primary button 44px+ high, solid, high contrast, directly under the form. "Forgot password?" small, right-aligned on the password label row. Social buttons below an OR divider, outlined, with their real brand colors.
- Copy says the plain thing: "Log in", not "Welcome back!". No sparkles, no exclamation marks.
- Submit: pressed state on the same frame, spinner only after ~300ms and held 500ms. Wrong password: field shakes once (0, -10, 10, -6, 6, -3, 0px over 360ms), keeps typed email, focus returns to the password field.

## Finish

Run `cross-cutting/design-review-checklist.md`. For motion details, run `procedures/polish/PROCEDURE.md`.
