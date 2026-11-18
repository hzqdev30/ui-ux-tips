# Backgrounds and Textures (make designs less flat)

22 background treatments that add depth to a flat design, plus the rules for using them without looking generated.

## When to use

- A page, hero, card or login screen feels flat or empty.
- A gradient shows banding or looks "digital".
- Choosing a background for a doorway screen (landing hero, login, empty state, confirmation).

Colors are in `color-system`. Dark backgrounds are in `dark-mode`. The deeper rules on when a field or material is allowed (the five-test tree, "materials must earn themselves") are in `charles/unslop/SKILL.md` pass 8, with code in `charles/unslop/references/effects.md` and `charles/unslop/references/visuals.md`.

## The 22 backgrounds

1. Felt texture
2. Fluted glass
3. Thermal gradients
4. Water ripples
5. Speckled graphite
6. Single-hue landscapes
7. Blueprint grids
8. Halftone
9. Grainy gradients
10. Grass texture
11. Dithered images
12. Paper texture
13. Contour lines
14. Cloud sky
15. Pixel mosaics
16. Lens distortion
17. Stippled gradients
18. Square-dot grids
19. Blurred photos
20. Iridescent shapes
21. Impressionist paintings
22. ASCII and pixels

## Film grain

Add a little noise over gradients. It removes banding (the ugly stripes) and makes the surface look less digital. Grain is the fix for a named problem, so use it on gradients, not as a trend layer over flat color.

## Rules for using them

- **One texture at most, and only for a reason.** Fix a named problem (banding, flatness, no depth) or carry the product's world. Texture on a flat color "because it looks nice" is decoration.
- **Match the treatment to the world.** Blueprint grids and contour lines suit technical or terrain products; felt, paper and grass suit warm physical ones; ASCII, pixels and dither suit editorial, retro or developer brands; iridescent and lens distortion only when the product means something by them.
- **Materiality: a texture needs a reason.** Privacy glass over a password field works because it hides something. Fluted glass needs a high-contrast subject behind it to refract, or it reads as a striped print. Frosted glass needs something meaningful behind it.
- **The UI on top stays quiet and legible.** Keep text at 4.5:1 over the background, measured on the real pixels. Dots, grids and lines must not compete with text.
- **Palette of at most three hues, taken from the product's world.** A two-stop wash is not a field.
- **Doorway screens only.** Working screens people stare at (apps, dashboards, settings) keep neutral surfaces; richness lives in the content.
- **Stock check.** At the real viewing size, could it come from an illustration pack or template gallery (layered flat hills, gradient suns, a dashed trail)? If yes, redo it.

## Quick match

| Need | Reach for |
|---|---|
| Gradient bands or feels digital | Film grain, grainy or stippled gradients |
| Soft photo needs structure | Halftone, square-dot grid |
| Terrain, routes, data worlds | Contour lines, blueprint grids |
| One focal object to radiate from | Water ripples, concentric rings |
| High-contrast subject behind glass | Fluted glass |
| Editorial, heritage, developer feel | Dithered images, pixel mosaics, ASCII and pixels |
| Warm, physical, handmade feel | Felt, paper, grass, speckled graphite |
| Atmosphere without a literal picture | Cloud sky, single-hue landscapes, blurred photos, impressionist paintings |

## Checklist

- [ ] The texture fixes a named problem or carries the product's world
- [ ] At most one texture layer, at most three hues
- [ ] Text over it still passes 4.5:1
- [ ] It is not on a working screen (app, dashboard, settings)
- [ ] Passes the stock check at the real viewing size
