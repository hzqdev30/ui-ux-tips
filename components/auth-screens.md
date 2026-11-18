# Auth Screens (Login, Sign-up, Password)

A clean, familiar login gets users in fast without distraction.

## When to use

- Designing a login, sign-up or create-account screen.
- Placing "Forgot password?" or social login buttons.
- Designing password creation with guidance.

General field behaviour (labels, placeholders, errors) is in `forms-and-inputs`. Button hierarchy is in `buttons-and-ctas`.

## 1. Login screen anatomy

Each element has one job:
- Logo, title ("Welcome back") and short subtitle
- Label above each field, with a placeholder example
- Email input, password input with a show/hide eye
- "Forgot password?" link
- Acceptance/remember-me checkbox
- Primary CTA (Login)
- "OR" divider, then social login buttons
- Register/login switch link ("Don't have an account? Register")

Follow the familiar layout (see Jakob's Law in `ux-laws`): rounded fields with icons, "Forgot password?" aligned to the right.

## 2. Forgot password link

- Essential, but must not steal attention from the primary action.
- Place it just above (right-aligned on the password label row) or just below the password field.
- Make it slightly smaller than body text with enough contrast.
- Available when needed, never distracting from logging in.

## 3. Labels and placeholders

- Use labels above fields; do not rely on placeholders as labels. Placeholders are only supplemental guidance. (Details in `forms-and-inputs`.)

## 4. CTA

- Minimum 44px touch target.
- The login button must contrast strongly with the background (a filled dark button, not an outlined or low-contrast one).
- Put the CTA at the bottom of the form, near the other critical links such as social logins, so it is the first thing users see.

## 5. Social login

- Social buttons reduce friction. Add them if possible.
- Balance placement: prominent enough to notice but not overshadowing the traditional login. Put them below the primary CTA, separated by an "OR" divider.
- Label them clearly with recognisable icons (Apple, Google, Facebook); a "Continue with ..." label is clear.
- Use outlined or light styling so they are visibly secondary to the main button.

## 6. Create account and password

- Use the functional color palette: the sign-up button is the primary action color, not red; red appears only on the invalid field and its message (see `color-system`).
- Password field gets a show/hide eye toggle.
- Show a strength meter (for example 4 segments with a "Strong" label) and a live checklist of requirements with checks: at least 8 characters, includes a number, includes a special character, includes an uppercase letter.
- Show the specific rule violated beneath the field ("Password must contain at least 8 characters").
- Place terms text ("By signing up you agree to our Terms of Service and Privacy Policy") close to the CTA, and an "Already have an account? Log in" link below the social options.
- The close X on a sign-up modal is neutral grey, not red.

## 7. Password creation: principles to apply

Definitions are in `design-principles-cheatsheet`. Applied here:
- Reward early, punish late: the strength progress moves as soon as the person types; the error message waits until they finish the field. Once an error shows, re-check on every keystroke so it clears when fixed.
- Inline validation: catch very common passwords (`Password1!`) as they are typed.
- Chunking: show a suggested password in small groups.
- Closure: let the strength outline close into one full shape when the password is strong, so no "weak/strong" label is needed.
- Continuity: use monospace so each dot morphs into its letter on show/hide.
- Redundancy gain: any sound matches a visible change on the same frame.
- Materiality: a privacy-glass texture over the field only because it hides something.
- Anthropomorphism (optional, brand permitting): a small character looks away when the password is shown.

## Checklist

- [ ] Labels above fields, example placeholders
- [ ] Forgot password aligned right, small, readable
- [ ] Primary CTA large, high-contrast, near social options
- [ ] Social options below an OR divider, visibly secondary
- [ ] Password has show/hide, strength meter and live requirements
- [ ] Red used only for errors
