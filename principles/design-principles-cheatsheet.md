# Design Principles Cheat Sheet

One-line definitions of the animation principles, UX laws and perception principles used to justify design decisions. Use this to name the principle behind a choice, then open the linked guide for exact values.

## When to use

- You need the short, quotable reason for a design choice ("Fitts's law: bigger, closer targets are faster to hit").
- Naming which principle each animation or interaction uses.
- Designing a password or sign-up flow (the second half of this file).
- Reviewing a UI against principles rather than taste.

Full rules with exact timings, curves and code: `procedures/ux-animation/PROCEDURE.md` (and its `references/recipes.md`, `references/techniques.md`). The ten core UX laws with diagnosis table: `ux-laws`.

## Animation principles (Disney's 12, applied to UI)

- **Squash and stretch:** things squish on impact and stretch in motion, which gives them weight.
- **Anticipation (wind-up):** a small pull back before the big move, so people see it coming.
- **Staging the focus:** direct the eye to one thing at a time.
- **Pose to pose:** set the key poses and let the browser fill in the frames between.
- **Follow through:** parts keep moving after the main body stops, then settle.
- **Slow in and slow out:** speed up and slow down, never move at a constant speed.
- **Moving in arcs:** move along curves, not straight lines.
- **Secondary action:** a small flourish that backs up the main action.
- **Snappy timing:** duration sets the feel, so keep UI animations under 300ms.
- **Exaggerated feedback:** push it past real so the moment lands.
- **Solid drawing in 3D:** give flat things depth and volume.
- **Overall appeal:** the sum of every detail, done with care.

## UX laws and behaviour rules

- **Fitts's law:** bigger, closer targets are faster to hit.
- **Bigger hit areas:** the clickable area can be bigger than it looks.
- **Hick's law:** more choices mean slower decisions.
- **Miller's law:** we hold about 7 things in mind at once, so chunk information.
- **Doherty threshold:** respond within 400ms or it feels slow.
- **Postel's law:** accept messy input, give back clean output.
- **Jakob's law:** people expect your app to work like the apps they already use.
- **Frequency of use:** the more often something is used, the less it should animate.

## Perception, trust and motion-meaning principles

- **Origin-aware:** popups should grow out of whatever you tapped, not the middle of the screen (each citation opens from its little number).
- **Layout stability:** nothing should jump around while it loads. Save the space for each paragraph first, then let the words fill in.
- **Labor illusion:** people trust a result more when they can see the work behind it, even if it takes longer (for example a pizza tracker). Use it for results people must trust; never fake the work.
- **Brushing and linking:** hover one thing and everything connected to it lights up somewhere else. Common in data viz, rare in chat apps; use it wherever two views show the same item.
- **Film grain:** a little noise over gradients removes banding and looks less digital (see `backgrounds-and-textures`).

## Password and sign-up principles (one worked example)

These eight principles come from a single password-creation screen. They apply to any input that guides someone toward a valid value.

- **Reward early, punish late:** progress shows up the second you type, but errors wait until you are actually done, so the form stops yelling at you.
- **Inline validation:** check as the person types, so a very common password like `Password1!` is caught right away instead of after submit.
- **Chunking:** show the suggested password in small groups so it is easy to read (same reason phone numbers have dashes).
- **Closure:** let an outline close into one full shape once the password is strong, so no "weak/strong" label is needed.
- **Continuity:** set the characters in monospace so each dot morphs into its letter instead of swapping.
- **Redundancy gain:** every sound matches something on screen, so people see and hear the same event at once.
- **Materiality:** privacy glass over a password field, because a texture should have a reason.
- **Anthropomorphism:** a small character that looks away when the password is shown.

### How the two "validation timing" rules fit together

- Show *positive* progress immediately (a segment fills, a requirement ticks).
- Show *negative* feedback (an error message) only when the person has finished the field, or when a clearly bad value (a known common password) is detected.
- Once an error is showing, re-check on every keystroke so it clears the instant it is fixed.

## Naming the principle

When you add or review an animation, write its principle next to it in a comment or note ("anticipation: 5% pull back, 100ms"). If you cannot name one, ask whether it should exist at all (`procedures/ux-animation/PROCEDURE.md`, question 1: Should it move?).
