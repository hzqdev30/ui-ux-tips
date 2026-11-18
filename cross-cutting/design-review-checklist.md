# Design Review Checklist

A five-minute visual QA pass to run before a design leaves your hands. Each item points to the skill that owns the rule.

## When to use

- Before sharing a design with a team, client or developer.
- When asked to "review", "critique" or "polish" a screen.
- As a last pass after finishing a layout.

## The six quick checks

1. **Align.** Drag a guide along every row and column; anything a few pixels off shows (for example a button 6px lower in one pricing card). -> `spacing-grid-alignment`
2. **Corners.** Match nested corners: inner radius = outer radius minus padding (20px card, 12px padding, 8px inner). -> `spacing-grid-alignment`
3. **Hierarchy.** Squint test: blur the screen or step back; the single most important action (for example "Pay now") should still stand out. -> `visual-hierarchy-and-clean-ui`
4. **Colors.** Count your grays. Use "Selection colors" to find near-duplicates (#6E6E6E, #707070, #737373...) and replace them with the token. -> `color-system`
5. **Copy.** Search the file for leftover template text such as "Title", "Button", "Text". -> `ux-writing-microcopy`
6. **Dark.** If the product has dark mode, flip to it. Logos and shadows break first. -> `dark-mode`

## Extra checks

### Icons
Stroke weight, optical size, corner style, fill consistency, alignment. -> `icons`

### Consistency
Same button styles, icons, casing and price formats everywhere. -> `visual-hierarchy-and-clean-ui`

### States
Every interactive element has default, hover, pressed, focused, loading and disabled states; every list has an empty state; errors and loading are designed. -> `buttons-and-ctas`, `feedback-states-and-dialogs`

### Touch and mobile
Tap targets at least 44px, primary action in the thumb zone. -> `mobile-ui-and-touch`

### Accessibility
Text contrast at least 4.5:1; no meaning conveyed by color alone. -> `color-system`

### Real content and testing
- Use real content early instead of lorem ipsum.
- Test designs with users; do not design in isolation. Borrow ideas, then test them with your users.

### Onboarding flows
Run the five review questions (reason to start, human tone, easier answers, reminder control, predictable offer). -> `onboarding-flows`
