[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 1 — Build the static game shell

**Milestone A — Foundations**

**Goal:** Create the visible product before making it move. A clear layout makes later debugging much easier.

**Build:**

- A page shell with a title/brand area, a scoreboard area, a large game area, control hints, and buttons for starting and pausing.
- A first visual style: background, accent colors, typography, spacing, and button states.
- A scoreboard that shows both players, the current level, and a way to read the score at a glance.
- A responsive first pass that still looks intentional at narrow widths.

**Concepts:** semantic HTML, accessible button labels, CSS custom properties, the box model, flexbox and grid, typography scale, spacing systems, hover and focus-visible states, clamp-based sizing, early media queries, contrast.

**Decisions:** What is your visual identity? What colors represent you and the bot? Is the scoreboard above, beside, or inside the playfield? How much chrome should surround the game?

**Done when:**

- The page looks like a game, even with no JavaScript behavior.
- All important elements are present and aligned.
- Tab order is sensible and focus is visible.
- Nothing important is clipped at a narrow window size.

**Stretch:** Add score pips, a difficulty meter, or a subtle background pattern.

**Watch out:** Designing too many menus before the core exists, low-contrast text, and relying on color alone to convey meaning.

---

**Navigation:** **Previous:** [Phase 0 — Set up a workspace you can trust](phase-00-setup.md) · **Next:** [Phase 2 — Set up the canvas and draw the field](phase-02-canvas-field.md)
