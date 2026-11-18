# Buttons and CTAs

Buttons are the product's conversation with the user: every tap deserves a reply.

## When to use

- Designing a button, button group, or button component.
- Deciding which action is primary on a screen, card or dialog.
- Writing or reviewing button labels.
- Choosing button placement on mobile, in forms, modals and cards.

Color of states is in `color-system`. Wording beyond buttons is in `ux-writing-microcopy`. Mobile touch sizing is in `mobile-ui-and-touch`.

## 1. Hierarchy

- Buttons must look tappable. Do not make users guess what is clickable; give clickable elements a fill, outline or clear link styling.
- One primary action per screen. Three filled buttons compete.
- Primary = solid fill, highest contrast (main action). Secondary = outline or light tint (normal action). Tertiary = text only (small action).
- Style shows importance; only the main action gets the strongest style. Example: outlined or text-only "Try" beside a filled "Buy".
- Never style two equal-weight actions as filled (for example "Add to cart" and "Wishlist" both filled). Make the secondary a ghost or icon button.

## 2. Size and padding

- Horizontal padding is twice the vertical padding (Y top and bottom, 2Y left and right). Tiny side padding looks bad and hurts readability.
- Reference spec: text button 40px high, 20px side padding, hug width. Icon button 40x40 with a 20px icon. Icon plus text: about 12px on the icon side, 4px gap, 20px on the text side (smaller icon-side padding gives better balance).
- Round icon-only buttons: small 44px (gap 32), medium 56px (gap 24), large 72px (gap 12).
- Label text: short, clear, one line. If it wraps, shorten it. Reference label style: semibold 16 / line height 20 / 1% letter spacing. Text size guides given for buttons: mobile 14-16, tablet 14-17, desktop 15-20.
- Touch targets: minimum 44px (44-48px with about 8px of space around). A 40px height is fine for mouse-driven desktop; use at least 44px for anything tapped.
- Contrast between label and fill: 4.5:1 (see `color-system`).

## 3. Radius

- Rounded corners are easier to notice and feel friendly; sharp corners feel serious. Pick one and use it everywhere.
- Reference ranges: sharp 0-2, slightly rounded 4-16, fully rounded (pill) 40+.
- A pill button inside a card needs a card radius that matches (see `spacing-grid-alignment`).

## 4. States and variants

- Design every state: default, hover, pressed, focused (visible ring), loading, disabled. A static button gives no feedback.
- Variants: text only, icon left, icon right, icon only.
- Build the button as one component with variant properties (type, state, destructive, badge) so a change updates every instance (Figma: Alt/Opt + Cmd + K to create a component).

## 5. Labels

- Say what happens. "Submit", "OK" and "Click here" make people guess. Use verb plus object: "Create account", "Subscribe".
- Test: if the label still makes sense on its own, it is good.
- Icon-only buttons need a label unless the symbol is universal (see `icons`).

## 6. Destructive actions

- Name the object and say what will happen, in a red label such as "Delete file". Avoid vague "Are you sure? OK / Cancel".
- Pair it with a clearly safe alternative: "No, keep it" (soft tint) and "Yes, delete" (red filled).
- Make the dangerous button look dangerous so nobody triggers it by accident. (Dialog layout is in `feedback-states-and-dialogs`.)

## 7. Placement

- Mobile: stack full-width buttons at the bottom within the thumb zone; primary at the bottom, secondary above it. Respect side margins.
- Forms: left-aligned below the form, primary first, then secondary. Place the CTA at the bottom of the form and near other key links such as social login.
- Modals and dialogs: actions bottom-right, secondary to the left of primary, close X top-right (follows the Z reading path).
- Cards: put "Buy now" as a full-width button at the bottom after the description, with the price in the header, not a small button in the title row.

## 8. Show that it is working

- On tap, swap the label for a spinner and a progressive label ("Placing order..."), block repeat taps, then show success.
- Silence feels broken; a spinner says "I heard you".

## Checklist

- [ ] Exactly one primary per screen/dialog
- [ ] Padding ratio 2:1 (horizontal:vertical)
- [ ] All states designed, including loading and disabled
- [ ] Labels use verb plus object, one line
- [ ] Destructive actions named and red
- [ ] Placement matches the context (mobile, form, modal, card)
