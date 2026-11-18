# UX Laws

Ten behavioural laws that explain how people perceive and use interfaces. Use them to justify a design decision or to diagnose a screen that "feels off". Each law states the principle, then what to do.

## When to use

- Reviewing a screen and you need a reason, not just an opinion.
- Deciding how many options, steps or items to show at once.
- Deciding where the most important action or content goes.
- A flow feels slow, confusing, or full of effort for the user.

Visual composition rules (hierarchy, whitespace, Z-pattern) live in `visual-hierarchy-and-clean-ui`. Spacing numbers live in `spacing-grid-alignment`. This skill is about human behaviour.

## The laws

### 1. Jakob's Law - familiarity
Users spend most of their time on other products, so they expect yours to work the same way.
- Use familiar patterns: a bottom tab bar with Home / Search / Notifications / Profile, a standard login form layout, right-aligned "Forgot password?" under the password field.
- Keep common icons recognisable and reuse expected interactions.
- Do not make users relearn basics for the sake of novelty.

### 2. Hick's Law - fewer choices, faster decisions
The more options shown, the longer the decision.
- Remove unnecessary options and group related ones.
- Recommend a default (for example a highlighted plan).
- Reveal advanced options later (progressive disclosure).
- Example: a 7-item dropdown with overlapping answers becomes 4 clear radio options.

### 3. Fitts's Law - size and distance of targets
Time to hit a target depends on how big it is and how far away.
- Make key actions large and put them in easy reach (bottom of a phone, thumb zone).
- Separate important actions clearly from neighbours.
- Avoid tiny, hard-to-hit targets such as a small hamburger icon in a far corner.
- Group related buttons together near the content they act on instead of scattering them.

### 4. Miller's Law - limited working memory
People process a limited amount of information at once.
- Break content into small, meaningful chunks and group related information.
- Use short sections and short steps.
- Example: a picker of 6 tiny options becomes 4 larger ones.

### 5. Law of Proximity - closeness means relatedness
Elements that sit close together are read as related.
- Keep labels next to their fields; use spacing to show relationships.
- Separate unrelated groups clearly and add section headers (for example "Personal information", "Billing address").
- Group a card's title, tag and badge in one header; keep a price next to its unit and billing note directly beneath it.
- Smaller gaps inside a group, larger gaps between groups.

### 6. Von Restorff Effect - the different item is remembered
When many items look alike, the one that differs is remembered.
- Highlight the primary action and the recommended option (a recommended pricing card gets a filled treatment while others stay outlined).
- Use contrast intentionally. If everything stands out, nothing does.

### 7. Serial Position Effect - first and last are remembered best
- Put the key items at the start and the important actions at the end.
- Lead with the strongest benefit.
- Do not bury essentials in the middle of a list or page.

### 8. Tesler's Law - complexity cannot be removed, only moved
Decide who absorbs the complexity: the product or the user. Prefer the product.
- Provide smart defaults, auto-fill, saved payment details and one-tap confirmation.
- Automate repetitive work and suggest addresses instead of asking for everything.
- Present unavoidable complexity in an organised way: card number on its own row, expiry and CVV side by side, account options in a separate titled group.

### 9. Doherty Threshold - respond fast and visibly
- Give instant feedback to every action.
- Show a loading state whenever a response is not immediate.
- Confirm progress and success ("Saving..." then "Saved successfully!").
- Never leave the user guessing whether something happened.

### 10. Peak-End Rule - judged by the best moment and the ending
People remember the most intense moment and how an experience ends.
- Invest in a successful onboarding, delightful milestones, clear confirmations and a smooth end of checkout.
- Make the end state useful (a helpful empty state after success).
- Design the peak. Design the end.

## More laws and principles

Postel's law, Frequency of use, Labor illusion, Brushing and linking, Origin-aware, Layout stability and the password-flow principles are defined in `design-principles-cheatsheet`. The extended set (Parkinson, Pareto, Zeigarnik, goal gradient, Occam, Prägnanz and more) with exact rules is in `charles/ux-animation/SKILL.md`.

## Quick diagnosis table

| Symptom | Likely law | First fix |
|---|---|---|
| Users hesitate on a screen | Hick | Cut or group options, set a default |
| Users miss or mis-tap a button | Fitts | Enlarge, move to thumb zone, add space |
| Form or page feels overwhelming | Miller | Chunk into sections or steps |
| Users misread what belongs together | Proximity | Tighten within-group spacing, widen between groups |
| Users overlook the main action | Von Restorff | Make one element visibly different |
| Product feels hard to learn | Jakob | Use the standard pattern |
| Users repeat taps or ask "did it work?" | Doherty | Add immediate feedback and loading state |
| Users do too much manual typing | Tesler | Add defaults, auto-fill, suggestions |
| Flow feels flat or forgettable | Peak-End | Strengthen the success moment and the ending |
