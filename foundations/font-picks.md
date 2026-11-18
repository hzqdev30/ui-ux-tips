# Font Picks by Vibe

A shortlist of typefaces grouped by the feeling they give, plus the fonts that now read as "AI-made". Pick the vibe from the product's character first, then the font.

## When to use

- Choosing a typeface for a new site, app or brand.
- A design looks generic or "AI-generated" and the font is a suspect.
- Pairing a UI font with a mono or display partner.

Type scale, weights and hierarchy are in `typography`. Anti-AI-look rules (one interface family, weights 400-500, sentence case) are in `procedures/unslop/PROCEDURE.md` (pass 5, Type).

## Picks by vibe

| Vibe | Fonts |
|---|---|
| Clean Swiss look | ABC Diatype, TWK Lausanne, Switzer, Saans, Areal, Strichpunkt Sans |
| Something friendly | Studio Feixen Sans, PP Mori, Aeonik, Degular, GT Walsheim, Circular |
| A bit of personality | Apfel Grotezk, Aktiv Grotesk, ABC Favorit, Familjen Grotesk, ABC Monument Grotesk, ABC Oracle |
| Techy feel (mono) | ABC Diatype Mono, Söhne Mono, GT America Mono, IBM Plex Mono, Commit Mono, Departure Mono |

## AI-looking fonts to skip

Geist, Space Grotesk, Bricolage Grotesque, Instrument Sans, JetBrains Mono, Space Mono.

These are not bad fonts. They are the default picks of generated UI, so they signal "a model made this". Skip them unless the user or an existing brand already uses one.

## How to apply

- Most fonts above are paid (Diatype, Lausanne, Aeonik, Söhne, GT, ABC, PP families). If the project cannot license one, choose the closest free font in the same vibe and say so. Do not silently fall back to a skipped AI-look font.
- Free or open fonts in the list (verify the licence before shipping): IBM Plex Mono, Commit Mono, Familjen Grotesk, Departure Mono, Switzer (Fontshare).
- One interface family plus at most one partner (for example a mono for code or numbers). A display face appears once.
- Pick the vibe from the product's character words (see the Direction step in `procedures/unslop/PROCEDURE.md`), never from what is trending.

## Checklist

- [ ] Vibe chosen from the product, then font chosen from that vibe
- [ ] Not one of the six AI-looking fonts (unless already the brand's)
- [ ] One interface family, at most one partner
- [ ] If the pick is paid and unlicensed, a free stand-in from the same vibe is named
