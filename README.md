# ui-ux-tips

A Claude Code skill: curated UI/UX rule guides plus four full design procedures, behind one entry point (`SKILL.md`).

- 25+ topic guides: UX laws, hierarchy, spacing, color, dark mode, typography, font picks, backgrounds and textures, icons, buttons, forms, auth and password UX, navigation, cards, pricing, dashboards, onboarding, mobile, UX writing, review checklist.
- `charles/`: four bundled procedures (unslop, polish, ux-animation, unreasonable-craft). See Credits.

## Install

```bash
npx skills add hzqdev30/ui-ux-tips -g
```

Or by hand:

```bash
git clone https://github.com/hzqdev30/ui-ux-tips ~/.claude/skills/ui-ux-tips
```

Start a new session, then ask for it by name: "use ui-ux-tips to review this login page".

## Credits and licensing

The `charles/` folder is a copy of four skills from [LemonFace0309/charles-skills](https://github.com/LemonFace0309/charles-skills) by Charles Liu, bundled here unchanged for convenience:

- `charles/unslop` - adapted from [unslop](https://github.com/heydamir/unslop) by Damir Sokolovsky, licensed CC BY 4.0, plus Emil Kowalski's unslop-design skill.
- `charles/polish` - built from Emil Kowalski's UI polish and animation skills and Josh Puckett's Interface Craft.
- `charles/ux-animation` - built on Disney's 12 principles of animation (Thomas and Johnston), userinterface.wiki by Raphael Salaja, Laws of UX by Jon Yablonski, Emil Kowalski's animation skill and Josh Puckett's Interface Craft.
- `charles/unreasonable-craft` - by Charles Liu.

The upstream repository does not state a license for these skills. All rights in them remain with their authors; they are not covered by any license of this repository. If an author objects, open an issue and the file will be removed.

Everything outside `charles/` (the topic guides and the index) is collected from design carousels and written up as rules.
