# Cards and Imagery

Images must carry meaning; cards must put the important thing first.

## When to use

- Designing a content, product or image card, or a carousel of cards.
- Choosing photos or illustrations.
- Placing text over an image.
- Handling long descriptions inside a card.

Pricing plan cards have their own skill: `pricing-cards`. Corner radius math and grid gaps: `spacing-grid-alignment`.

## 1. Imagery

- Use images that support the story or meaning. A bill-payment screen should show an illustration of a card or payment, not a random wallet stock photo.
- Use crisp, high-resolution assets. A blurry or pixelated graphic is a quality error.
- Overlap elements to create depth and clarity: an avatar partly over a cover image, or stacked overlapping avatars, instead of flat, separated pieces.

## 2. Text over images

- Text on a bright photo is unreadable. Add a dark gradient overlay behind the text.
- For a more polished look use a linear (progressive) blur: the image gets blurrier toward the bottom behind the text, so text stays readable while the image stays vivid. It looks softer than a plain linear gradient.

How to build linear blur in Figma:
1. Create a frame for the card (website example 440 x 580).
2. Apply a background image (for example from an Unsplash plugin).
3. Create a smaller rectangle with the same width and enough height for the text (440 x 200).
4. Duplicate it. On one copy add a linear gradient (same color, 0% opacity to 100% opacity). On the other set the fill to about 1% and add a Background blur effect (blur about 20).
5. Put the blur shape behind the gradient shape, select both and use as mask.
6. Drop it into the image frame at the bottom and add the text on top.
7. Tune fill color, gradient stop positions and blur amount (lighter fill plus stronger blur, or darker fill plus lighter blur) until the transition feels right.

## 3. Long text in cards

- Truncate after a few lines (for example five) with an ellipsis and a "Read more" link or button. Do not let long text stretch the card or force inner scrolling.

## 4. Product card layout

- Put the product name and price together at the top of the content, with the price more prominent (larger or in the accent color), instead of a small price tucked below the description.
- Put the buy action as a full-width button at the bottom of the card after the description, not as a small button in the title row.
- A wishlist heart is a secondary action: an icon on the image corner, not a second filled button.
- Keep button style, icons, casing and price format identical across all cards.

## Checklist

- [ ] Every image supports the content
- [ ] No low-resolution assets
- [ ] Text over images has an overlay, gradient or blur and is readable
- [ ] Long descriptions truncated with Read more
- [ ] Price prominent; primary action at the card bottom
