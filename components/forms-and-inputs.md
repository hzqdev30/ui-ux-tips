# Forms and Inputs

Make forms short, clear and forgiving.

## When to use

- Designing or reviewing any form (contact, checkout, payment, profile, booking).
- Deciding label and placeholder behaviour.
- Writing validation and error behaviour.
- Building multi-step forms or search with suggestions.

Login/sign-up specifics are in `auth-screens`. Choice controls (radio, checkbox, slider, toggle) are in `selection-controls`. Wording of error messages is in `ux-writing-microcopy`.

## 1. Labels and placeholders

- Put the label above the input. Do not use the placeholder as the label: it disappears as soon as the user types, which causes confusion.
- Use placeholders only for supplemental guidance, never for critical information.
- Placeholder should show an example format ("Example@gmail.com"), not repeat the label ("Enter Email").
- Differentiate the three text states: label (strong, above), placeholder (light grey), entered value (dark). If placeholder and value look identical, users cannot tell what is filled.

## 2. Keep the number of fields minimal

- Replace separate Day / Month / Year dropdowns with one date field with a format hint (DD/MM/YY) and a calendar icon. Use a single time field instead of hours / minutes / AM-PM dropdowns.
- Use a single email field, not a split "address @ domain" pair.
- For long lists of radio options, show the main ones plus an "Other" option instead of every possibility.
- Use input masks to guide entry: a date mask such as dd/mm/yyyy, a phone mask such as (+___) __ ___ ___.

## 3. Group fields by relationship

- In long forms group related inputs: expiry and CVV side by side on one row, card number on its own row, phone number separate.
- Do not stack every field in one column with short fields orphaned on their own lines.
- Titled groups (for example "Card details" and "Account details" as separate cards) clarify structure. (Proximity logic: `ux-laws`.)

## 4. Validation and error messages

- Show the error at the field that caused it: red border plus an icon on the field and a message directly beneath it ("Please enter a valid card number"). Do not list errors together at the bottom or in a generic banner.
- Validate quickly, in real time where sensible, so users can fix an error before moving on.
- Say how to fix it in plain language; do not blame the user ("Invalid password" becomes "Password must be at least 8 characters, include a number and a capital letter").
- Show success states too: green border plus a check, no message text ("Looks good!" is banned, see the resolved conflicts in `SKILL.md`).
- Error color is reserved for errors only (see `color-system`).

## 5. Multi-step forms: show progress

- Add a stepper at the top showing done (check), current (highlighted) and upcoming (grey) steps with labels (Address, Payment, Review).
- Provide Back (secondary) and Continue (primary).
- Benefit: sets expectations, reduces uncertainty, helps people finish.

## 6. Autocomplete

- Suggest results as users type: bold or highlight the matching part and highlight the first suggestion.
- Benefit: less typing, faster navigation, relevant results quickly.

## Checklist

- [ ] Labels above fields; placeholders only give examples
- [ ] Placeholder, value and label visually distinct
- [ ] Fewest possible fields; masks and single date/time/email fields
- [ ] Related fields grouped; short fields share rows
- [ ] Errors appear beside their field and explain the fix
- [ ] Multi-step forms show progress
