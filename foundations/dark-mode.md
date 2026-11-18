# Dark Mode

Dark mode is easier on the eyes only when applied correctly. It is not an inversion of the light theme.

## When to use

- Adding a dark theme to a product.
- Converting a light design to dark.
- Choosing background color, surface elevation, or shadow treatment on dark surfaces.
- Reviewing a dark screen for contrast and eye strain.

General palette logic is in `color-system`. This skill covers only what changes in dark mode.

## 1. Background color

- Default to `#121212`. Google recommends it and warns that pure black (`#000000`) creates too high a contrast.
- Pure black is a valid, deliberate choice on iOS: Apple uses `#000000` in its dark mode (YouTube uses about `#222222`).
- Recommended default for new designs: `#121212`. Use `#000000` only when matching the iOS system look on purpose.

## 2. Elevation

- Elevate a surface by overlaying white at different opacities. Reference levels: 8%, 12%, 16% white on the background (higher elevation, higher opacity).
- Do not elevate with fancy shadows or with different arbitrary dark shades.

## 3. Color and saturation

- Use less saturated, lighter versions of brand colors. Highly saturated colors against dark surfaces cause eye strain and vibrate.
- Do not reuse the exact light-mode colors in dark mode. The same saturated colors read differently on dark and light backgrounds; tune each color per mode (for example a slightly different tone on dark) so it stays balanced.

## 4. Shadows

- Do not invert shadows. A black shadow turned white becomes a glow and looks cheap and strange.
- Express depth through the white-overlay elevation levels above instead.

## 5. Accessibility first

- Contrast is the biggest trap of dark mode. Dark grey text on a dark background is unreadable; use light, high-contrast text.
- Check text and icon contrast against the actual surface they sit on, including elevated surfaces.

## 6. Verify before sharing

- Flip the design to dark if the product has a dark theme. Logos and shadows break first (a dark logo vanishes on a dark background).

## Checklist

- [ ] Background is `#121212` (or deliberately `#000000` for iOS)
- [ ] Elevation uses white overlays, not shadows or random dark shades
- [ ] Colors are desaturated for dark and tuned per mode
- [ ] No inverted shadows
- [ ] Text and icon contrast verified on every surface
- [ ] Logos and imagery checked on dark
