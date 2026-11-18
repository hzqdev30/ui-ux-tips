# Settings and Profile Screens

Settings are where users go to control the product. Make them scannable, plainly worded and safe.

## When to use

- Designing or reviewing settings, preferences, account or profile screens.
- Deciding how to organise a long list of options.
- Designing account deletion, data export or privacy controls.

Toggle behaviour is in `selection-controls`. Confirmation dialog structure is in `feedback-states-and-dialogs`. Early preference capture is in `onboarding-flows`.

## 1. Organise

- **Group settings into categories** that make sense to users, not to the code structure. Put each group in its own container with a label (for example Security, General, Legal), and keep account actions (log out, close account) together.
- **Visual hierarchy**: smaller gaps inside a group, larger gaps between groups. Settings should be scannable at a glance.
- Use a chevron on items that open another screen; place toggles directly in the list so users can switch them without leaving the screen.

## 2. Labels and descriptions

- Use plain-language labels that say what the setting does. Avoid technical or marketing names that only the team understands.
- Add a short description to complex settings ("Display & Brightness" tells people what they will find; "Profile details - manage your personal information").
- Examples of rewrites: Conditions becomes Terms and conditions; Questions becomes Help and support; Delete becomes Close account; Leave app becomes Log out; Balances toggle becomes Hide balances.
- Add universally understood icons next to labels as a scanning aid (see `icons`).

## 3. Surface what matters

- **Highlight critical settings.** Frequently used settings must be easy to find; do not bury key functions five levels deep just to look tidy. Give key options larger icons, extra context (subtitle) and the current value on the right (Currency: USD, Plan: Yearly).
- **Secondary actions**: keep the most-used items on the first screen; push the rest into subpages so not everything is shown at once.
- **Progressive settings**: start with the basics, then let users reach more. Three levels: (1) base settings, (2) data and additional options, (3) rarely changed advanced options in an edit screen with Cancel and Save.

## 4. Placement and search

- Put profile/settings where users expect it: in the tab bar, or behind the avatar image (tap the avatar in the header). In complex apps put it in the tab bar as a "More" item (see `navigation`).
- Add a search field when a list is longer than about 6-8 items. Typing a keyword beats clicking back and forth.

## 5. Personalization and profile details

- Optional but valuable: address users by name, let them upload an avatar, and show personalised offers as dismissible cards.
- Show verified information as read-only and flag unverified items with a clear prompt ("Verify this email").
- Explain why you need sensitive information ("We need this information to verify your identity").
- Detail screens can offer copy buttons for account details.

## 6. Edge cases: delete, export, privacy

- These need extra care: make the action clear but hard to trigger accidentally.
- Use an attention-grabbing warning visual (red warning icon), a distinct button style (outlined red "Yes, delete my account"), a plain explanation of consequences and exceptions, and a final confirmation dialog before the action completes.

## Checklist

- [ ] Settings grouped and labelled; gaps larger between groups
- [ ] Plain labels, descriptions for complex items
- [ ] Frequent settings up front, advanced behind progressive levels
- [ ] Search present for long lists
- [ ] Profile/settings in an expected location
- [ ] Destructive/privacy actions distinct and confirmed
