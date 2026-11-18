# Mobile UI and Touch

Design for thumbs, not cursors.

## When to use

- Designing or reviewing mobile screens.
- Choosing tap target sizes and spacing between tappable items.
- Placing primary actions for one-handed use.
- Picking mobile margins and gaps.

Tab bar internals are in `navigation`. General spacing scale is in `spacing-grid-alignment`. Button anatomy is in `buttons-and-ctas`.

## 1. Touch targets

- Minimum 44px for anything tappable (44-48px height with about 8px of space around so neighbours are not hit by mistake).
- Do not shrink secondary controls too far. A tiny dismiss "x" next to a Follow button needs a larger tap area and icon.
- Make whole rows tappable (checkbox plus label), not just a small box. (See `selection-controls`.)

## 2. Thumb zone

- Key actions go in easy reach at the bottom of the screen.
- Stack full-width buttons at the bottom with the primary at the very bottom; small centered buttons look incomplete on mobile. Respect system-specific margins.
- Avoid placing key controls in far corners (a small hamburger at the top corner is hard to reach).

## 3. Mobile spacing values (from the sources)

| Where | Value |
|---|---|
| Side margins (screen edge to content) | 24px |
| Title to its content | 16px |
| Between sections | 24 or 32px |
| Between tabs/chips and between cards (horizontal) | 8 or 12px |
| Between buttons | 12px |

- A gap of 8-12px between horizontally scrolling cards or tabs keeps them balanced and makes it visible that more content extends beyond the screen.

## 4. Text on mobile

- Interface text around 14-16pt (button text guidance: mobile 14-16, tablet 14-17, desktop 15-20).
- Keep button labels on one line; shorten them if they wrap.

## 5. Lists and long text

- Truncate long descriptions with "Read more" instead of making users scroll within a card (see `cards-and-imagery`).
- Use skeleton loading rather than a spinner on a blank screen (see `feedback-states-and-dialogs`).

## Checklist

- [ ] All tap targets at least 44px with space around
- [ ] Primary action reachable by thumb
- [ ] Side margin 24px, consistent section gaps
- [ ] Full-width buttons respect margins
- [ ] No tiny dismiss or close controls
