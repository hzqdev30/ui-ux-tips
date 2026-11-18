# Selection Controls

Pick the control that fits the choice, and make state obvious.

## When to use

- Deciding between radio, dropdown, checkbox, chips, toggle, slider.
- Designing a checkbox list or multi-select.
- Designing filters.
- Making selected/unselected state clear.

Text input behaviour is in `forms-and-inputs`. Number of options and decision speed (Hick's Law) is in `ux-laws`.

## 1. Checkboxes (4 rules)

1. **Make checkboxes look like checkboxes.** A square box with a check mark is read as a checkbox. Round boxes (read as radio buttons) or "+" and "x" icons confuse people.
2. **Lay long lists out vertically.** Do not wrap them in horizontal rows. Give the group a label ("Select days").
3. **Use chips when vertical space is limited.** Pill-shaped toggles with a check icon when selected work as a compact alternative.
4. **Make the clickable area large**, especially on mobile: the whole row (box plus label) should be tappable, not only the tiny box.

## 2. Radio vs dropdown

- For a short list (about 4 options) show radio buttons so all options are visible, rather than a long dropdown (a 7-item dropdown with overlapping answers is worse).
- Trim redundant options; if the list is long, show the main options plus an "Other" choice.

## 3. Sliders in filters

- Use a dual-handle range slider with visible values instead of two separate From / To number inputs. It is faster and shows the range at a glance.

## 4. Toggles

- A toggle switch gives an immediate on/off setting. Placing key toggles directly on the main settings screen allows quick personalization and saves time.
- Give a toggle a short description when the effect is not obvious ("Public profile - select to make profile visible to others").
- When several toggles control similar items (morning / day / evening reminders), give each its own time and switch.

## 5. Selected state must be visible

- Show selection with a filled color and a check mark; selected answers should remain visible as the user moves forward.
- Use one color to mean "selected" (grey for unselected). See `color-system`.
- When multi-select is limited, say so ("Choose up to 3").

## Checklist

- [ ] Control type matches the choice (one-of-few: radio; many: dropdown/search; any-of: checkbox)
- [ ] Checkbox is a square with a check; full row tappable
- [ ] Lists vertical, group labelled; chips if space is tight
- [ ] Ranges use a slider with values
- [ ] Selected state uses fill plus check, one consistent color
