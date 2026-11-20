# Dashboards and Data Visualisation

A dashboard answers one question for one person, fast: "what needs me right now?" Everything on it either answers that or goes.

## When to use

- Designing a dashboard, home screen, analytics screen or admin landing page.
- Laying out stat figures, a main chart and lists.
- Choosing a chart type for a dataset.

Sidebar spacing is in `spacing-grid-alignment`; navigation in `navigation`; restraint and hierarchy in `visual-hierarchy-and-clean-ui`. Generic-dashboard tells and their fixes are in `procedures/unslop/references/signs.md`; starting sizes are in `procedures/unslop/references/tokens.md` (App layout). For a dashboard inside an app with house components, also read `cross-cutting/component-systems`.

## 1. Start from the job, not the layout

Before drawing anything, write three lines:

1. **Who opens it, and when.** "The duty clerk, at the start of a shift and between bookings."
2. **The question it answers.** "Which halls are free this week, and who is coming in today?"
3. **What they do next.** "Take a booking for a free slot; check in today's hirer."

Then every block must serve line 2 or line 3. A widget that only "shows data" (a traffic line chart nobody acts on, a doughnut of route shares) is cut.

## 2. Structure

1. **Page title is the period or the place, not a greeting.** "Jumaat, 20 November" or "Today", never "Welcome back, Aina!".
2. **Context line under it** when the job depends on it: duty officer, weather, which branch, last sync. One line, no cards.
3. **The one primary action** in the header, top-right on desktop, in reach on a phone ("Tempah slot", "Post notice"). Only one.
4. **Stat figures (optional).** 3 or 4 compact figures, one row, one height. Each is a number, its label and its change *against something* ("+3 vs last week"). No icons, no sparklines, no mini bars inside them.
5. **One main block** that shows the real work, at least two thirds of the width: a timeline, a calendar, a queue, a map, the main chart. It is the moment of the screen (`procedures/unslop` pass 8: real content, drawn with care).
6. **One secondary block** beside or below it: a list of what needs attention, today's items, approvals waiting. A list or table, not a second chart.
7. **Full list or table** below, if the job needs it.

There is no fixed grid of equal widgets. Size each block by how much it matters; the main block gets the room.

## 3. Rules

- **Do not wrap everything in identical cards.** A card is for a group that needs a boundary. Stat figures can share one surface; the page title and context line never sit in a card. Nested cards are never allowed.
- **Card and section headings carry no icon by default.** The title is enough. An icon earns its place only when it carries meaning a word would not (a status, a warning).
- **Repetition is noise.** If every cell says the same word ("Tidak tersedia" 21 times), show the exception, not the rule: draw free slots and leave unavailable ones as quiet empty space, with a legend once.
- **Labels once.** Column headers (Pagi, Petang, Malam) appear once at the top, not in every row.
- **Status never by colour alone.** Pair colour with a word, an icon or a fill pattern.
- **Numbers:** `tabular-nums`, one format across the screen, units stated once.
- **Empty is a state, not a hole.** An empty "today" block is one line plus the action ("No bookings today. [Take a booking]"), sized to its content, not a tall card with a big grey icon.
- **Design with realistic data.** Before judging a dashboard, load data that looks like a real busy day (some booked, some free, one late, one cancelled). A dashboard judged empty always looks unfinished.
- **Brushing and linking** where two blocks show the same item: hover a row, highlight its slot (`principles/design-principles-cheatsheet`).
- **Finished things recede.** Past slots and completed items go quiet (muted fill), so what is left stands out.

## 4. Scanning

People scan the top edge, then down the left. Put the answer to the job's question along the top and left: the title and context, then the main block. Secondary information goes right or below.

## 5. Pick the chart by purpose

| Purpose | Chart options |
|---|---|
| Change over time | Line, column, timeline |
| Comparison | Bar (horizontal when labels are long), column |
| Part of a whole | Stacked bar; a pie only for 2 or 3 parts, with values printed |
| Distribution | Histogram, dot plot |
| Schedule or capacity | Timeline lanes, calendar grid |

One or two series per chart, muted grid lines, one highlight colour for the thing that matters, the rest in neutral steps. No rainbow series, no glowing or pill-shaped bars, no doughnut just to fill a slot.

## Checklist

- [ ] The job's three lines are written, and every block serves them
- [ ] Title is the period or place, not a greeting
- [ ] One primary action, top-right or in reach
- [ ] Stat figures (if any) are number + label + compared change, no icons or sparklines
- [ ] One main block takes the room; the second block is a list, not another chart
- [ ] No identical card grid, no icon on every heading, no nested cards
- [ ] Repeated words and labels removed; empty states are one line plus an action
- [ ] Judged with realistic data, at 360 px and 1440 px
