# Font Picks by Vibe

A shortlist of typefaces grouped by the feeling they give, plus the fonts that now read as "AI-made". Pick the vibe from the product's character first, then the font.

## When to use

- Choosing a typeface for a new site, app or brand.
- A design looks generic or "AI-generated" and the font is a suspect.
- Pairing a UI font with a mono or display partner.

Type scale, weights and hierarchy are in `typography`. Anti-AI-look rules (one interface family, sentence case) are in `procedures/unslop/PROCEDURE.md` (pass 5, Type).

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

## Every project picks a font

The system font (`system-ui`, Segoe UI, Arial) reads as "nobody chose". Every project picks an interface font, and optionally a mono partner, once at setup, and records the choice where the team keeps design decisions. Use the system font only when the user decides it (for example, a strict no-download rule).

How to install it, by project type:

| Project | Install | Load |
|---|---|---|
| Vite, Laravel, React, any npm build | `npm i @fontsource/<font>` for Google/Fontsource fonts (see `font-sources`) | In the main CSS: `@import "@fontsource/<font>/400.css";` and `500.css`, then set `--font-sans` |
| Fontshare or GitHub-only fonts (Switzer, Satoshi, Overused Grotesk) | Download the zip from `font-sources`, copy the `.woff2` files and the licence into the project (for example `resources/fonts/`) | `@font-face` in the main CSS, `font-display: swap` |
| Plain HTML prototype | The CDN links in `font-sources.css` | A `<link>` in the page |

A project that forbids CDNs still gets a real font: install it through npm or self-host the files. Load only the weights you use (usually 400 and 500).

## Free stand-ins and downloads

Free fonts for each vibe, with licence and download link, are in `font-sources` (and a ready CSS file, `font-sources.css`). Free stand-ins by vibe: Swiss = Switzer, Overused Grotesk, BDO Grotesk, Host Grotesk, Giphurs; friendly = Satoshi, General Sans, Funnel Sans; personality = Apfel Grotezk (the real one), Familjen Grotesk, Lil Grotesk, Cabinet Grotesk; mono = IBM Plex Mono, Commit Mono, Departure Mono, Intel One Mono, Server Mono.

## How to apply

- Most fonts above are paid (Diatype, Lausanne, Aeonik, Söhne, GT, ABC, PP families). If the project cannot license one, choose the closest free font in the same vibe and say so. Do not silently fall back to a skipped AI-look font.
- Free fonts on the list: IBM Plex Mono, Commit Mono, Familjen Grotesk, Departure Mono, Switzer, Apfel Grotezk. Links in `font-sources`.
- One interface family plus at most one partner (for example a mono for code or numbers). A display face appears once.
- Pick the vibe from the product's character words (see the Direction step in `procedures/unslop/PROCEDURE.md`), never from what is trending.

## Checklist

- [ ] A font was chosen and installed (not the system font, unless the user decided so)
- [ ] Vibe chosen from the product, then font chosen from that vibe
- [ ] Not one of the six AI-looking fonts (unless already the brand's)
- [ ] One interface family, at most one partner
- [ ] If the pick is paid and unlicensed, a free stand-in from the same vibe is named
