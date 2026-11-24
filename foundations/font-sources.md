# Font Sources (download map)

Where every font in `font-picks` and the Selat Line comparison page comes from, so a new project can get the same font without searching again. Every font here is free for commercial use, with no trial limits (checked 2026-11-18). Cal Sans was removed: it ships one heavy weight and does not suit an interface font.

## When to use

- Starting a project and you picked a font from `font-picks` or the comparison page.
- You need the real files (self-hosting) or an install command.

Picking a font by vibe is in `font-picks`. Type sizes and weights are in `typography`.

## Fastest way to use any of them

Copy `font-sources.css` (next to this file) into the project and link it. It loads every font below, with the exact versions that were tested. Then set the family:

```css
:root { --font-sans: "Switzer", system-ui, sans-serif; --font-mono: "IBM Plex Mono", ui-monospace, monospace; }
```

For production, load only the one or two fonts you use, and self-host them (download the files, keep the license file beside them, use `font-display: swap`). `font-sources.css` pulls everything, so it is for trying fonts, not for shipping.

## Map

| Font | Style | Weights | License | Official page | Download | npm package |
|---|---|---|---|---|---|---|
| Switzer | Swiss | 400, 500, 600, 700, 800 (the template needs 700 and 800) | Fontshare free licence | [Fontshare](https://www.fontshare.com/fonts/switzer) | [zip](https://api.fontshare.com/v2/fonts/download/switzer) | - |
| Satoshi | Friendly | 400, 500, 600 (more in the zip) | Fontshare free licence | [Fontshare](https://www.fontshare.com/fonts/satoshi) | [zip](https://api.fontshare.com/v2/fonts/download/satoshi) | - |
| General Sans | Friendly | 400, 500, 600 (more in the zip) | Fontshare free licence | [Fontshare](https://www.fontshare.com/fonts/general-sans) | [zip](https://api.fontshare.com/v2/fonts/download/general-sans) | - |
| Cabinet Grotesk | Personality | 400, 500, 600 (more in the zip) | Fontshare free licence | [Fontshare](https://www.fontshare.com/fonts/cabinet-grotesk) | [zip](https://api.fontshare.com/v2/fonts/download/cabinet-grotesk) | - |
| Overused Grotesk | Swiss | 300-900 variable | SIL OFL | [GitHub](https://github.com/RandomMaerks/Overused-Grotesk) | repo `fonts/` folder | - |
| BDO Grotesk | Swiss | Light to Black (static) | SIL OFL | [GitHub](https://github.com/LCTipografi/BDO-Grotesk) | repo `Fonts/` folder | - |
| Giphurs | Swiss | ExtraLight to Black (static) | SIL OFL | [GitHub](https://github.com/Corne2Plum3/Giphurs) | repo `fonts/` folder | - |
| Lil Grotesk | Personality | 100-900 variable | SIL OFL | [GitHub](https://github.com/noirblancrouge/LilGrotesk) | repo `fonts/` folder | - |
| Apfel Grotezk | Personality | Regular 400, Mittel 500, Satt 600, Fett 700 (+ Brukt) | SIL OFL | [Collletttivo](https://www.collletttivo.it/typefaces/apfel-grotezk) | [GitHub](https://github.com/collletttivo/apfel-grotezk) `fonts/` (woff2 included) | - |
| Host Grotesk | Swiss | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Host+Grotesk) | Download family button on the Google page | `npm i @fontsource/host-grotesk` |
| Funnel Sans | Friendly | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Funnel+Sans) | Download family button on the Google page | `npm i @fontsource/funnel-sans` |
| Familjen Grotesk | Personality | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Familjen+Grotesk) | Download family button on the Google page | `npm i @fontsource/familjen-grotesk` |
| IBM Plex Sans | Baseline | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Sans) | Download family button on the Google page | `npm i @fontsource/ibm-plex-sans` |
| Inter | Baseline | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Inter) | Download family button on the Google page | `npm i @fontsource/inter` |
| Geist | AI-looking, skip | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Geist) | Download family button on the Google page | `npm i @fontsource/geist` |
| Space Grotesk | AI-looking, skip | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Space+Grotesk) | Download family button on the Google page | `npm i @fontsource/space-grotesk` |
| Instrument Sans | AI-looking, skip | 400-600+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Instrument+Sans) | Download family button on the Google page | `npm i @fontsource/instrument-sans` |
| Commit Mono | Mono | 400, 700 + more | MIT/OFL | [commitmono.com](https://commitmono.com) | [v1.143 zip](https://github.com/eigilnikolajsen/commit-mono/releases/download/v1.143/CommitMono-1.143.zip) | `npm i @fontsource/commit-mono` |
| Departure Mono | Mono | 400 only (pixel font) | MIT/OFL | [departuremono.com](https://departuremono.com) | [v1.500 zip](https://github.com/rektdeckard/departure-mono/releases/download/v1.500/DepartureMono-1.500.zip) | - |
| Server Mono | Mono | 400 only (+ oblique) | SIL OFL | [GitHub](https://github.com/internet-development/www-server-mono) | repo `public/fonts/` | - |
| IBM Plex Mono | Mono | 400-500+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Mono) | Download family button on the Google page | `npm i @fontsource/ibm-plex-mono` |
| Intel One Mono | Mono | 400-500+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Intel+One+Mono) | Download family button on the Google page | `npm i @fontsource/intel-one-mono` |
| Geist Mono | Mono, baseline | 400-500+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Geist+Mono) | Download family button on the Google page | `npm i @fontsource/geist-mono` |
| JetBrains Mono | Mono, AI-looking, skip | 400-500+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/JetBrains+Mono) | Download family button on the Google page | `npm i @fontsource/jetbrains-mono` |
| Space Mono | Mono, AI-looking, skip | 400-500+ (Google Fonts) | SIL OFL | [Google Fonts](https://fonts.google.com/specimen/Space+Mono) | Download family button on the Google page | `npm i @fontsource/space-mono` |

Notes:
- Fontshare zips come from `api.fontshare.com/v2/fonts/download/<slug>`; each has a license file.
- Google Fonts and Fontsource packages carry the OFL license text; keep it when self-hosting.
- Apfel Grotezk on Fontsource has only 400 and 700, so `font-sources.css` loads all four weights from the author's GitHub repo instead.
- GitHub-hosted fonts are pinned to a commit hash inside `font-sources.css` so the files cannot change under you.
- Weight rule from the skill: use 400-500, 600 for rare emphasis (a project built on a template uses the weights the template pages use, usually 500-700, so install a family that has them); a single-weight font is fine for small mono text, but pick one with a real 500 for headings.

## Paid originals (no free version exists)

ABC Diatype and Diatype Mono, TWK Lausanne, Saans, Areal, Strichpunkt Sans, Studio Feixen Sans, PP Mori, Aeonik, Degular, GT Walsheim, Circular, Aktiv Grotesk, ABC Favorit, Monument Grotesk, ABC Oracle, Söhne Mono, GT America Mono. Some have free trial fonts for mockups only; they need a licence for real products. Use the free stand-ins above.
