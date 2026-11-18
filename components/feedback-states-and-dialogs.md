# Feedback States and Dialogs

Never leave the user guessing. Every state - empty, loading, error, success, risky - needs a deliberate design.

## When to use

- A screen or list can be empty.
- Designing loading, error, no-results or success states.
- A destructive or irreversible action needs confirmation.
- Deciding between a modal, a banner, a toast or inline feedback.

Field-level validation is in `forms-and-inputs`. Alert colors and banner styling are in `color-system`. Button labels for dialogs are in `buttons-and-ctas`. Response-time principle: `ux-laws` (Doherty).

## 1. Empty states

- Treat an empty state as an opportunity, not a blank. Use an icon or illustration, a headline ("No items yet"), helpful sub-copy ("Your saved items will appear here") and a call to action ("Explore products").
- Set the right expectation, reassure, and point to the next best action (for example "No investments yet" with a primary "Explore Mutual Funds").
- Friendly or playful tone is welcome; a bare "Basket is empty" is not.

## 2. Error and no-results states

- Turn errors into helpful moments: illustration, clear message ("We couldn't find any results"), guidance ("Try checking your spelling or different keywords"), a primary action ("Search again") and a secondary one ("Browse popular topics").
- Reduces frustration and keeps users engaged by giving a clear next step.
- System-level errors can use an error banner ("Something went wrong. Please try again.").

## 3. Loading

- Use skeleton screens instead of a spinner on a blank page: grey placeholder blocks that mirror the final layout reduce perceived waiting time and show that content is coming.
- Show progress for long tasks (for example download percentage with a cancel control).
- Confirm completion: "Saving..." then "Saved successfully!".

## 4. Toasts and banners

- Use a toast for short, non-blocking confirmations ("Changes saved") with a close control.
- Use a banner for persistent system messages. Match style to meaning: info, warning, success, error (see `color-system`).

## 5. Tooltips

- Give quick, contextual help without leaving the screen: an "i" icon next to the label that opens a short tooltip with a title and brief explanation.
- Keeps the interface clean and provides information on demand. If a tooltip is needed to explain an icon, add a label instead (see `icons`).

## 6. Confirmation dialogs and destructive actions

- Use them for important or irreversible actions so users can reconsider; they prevent accidental loss.
- Structure: a warning icon, a title that names the object ("Delete this item?"), a plain explanation ("This action cannot be undone"), and two buttons - a safe secondary (Cancel / "No, keep it") and a clear destructive primary ("Yes, delete").
- For very serious actions (account deletion): make the entry point visually distinct (red warning illustration, outlined red button), explain consequences and exceptions, and require an extra confirmation before the final action. Make the action clear but hard to trigger by accident.

## 7. Do not overuse popups

- A modal over a dimmed page for something minor (like a rating request) interrupts users. Prefer inline feedback, such as a rating row at the bottom of the content.

## Checklist

- [ ] Every list/screen has an empty state with a next step
- [ ] Errors say what happened and what to do
- [ ] Skeletons for page/list loads; progress for long tasks
- [ ] Success confirmed
- [ ] Destructive actions named, confirmed, and visually distinct
- [ ] Popups reserved for important interruptions
