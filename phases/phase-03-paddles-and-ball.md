[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 3 — Give the game state a shape: paddles and ball

**Milestone A — Foundations**

**Goal:** Represent the game objects as data and draw them from that data.

**Build:**

- Game state for the human paddle, the bot paddle, and the ball: position, size, and any motion values you expect to need.
- A scene with two paddles and a ball in believable starting positions.
- Visual styling for each object that fits your theme.
- One authoritative place that draws the current state.

**Concepts:** objects as state containers, coordinates: center versus top-left, rectangles, circles, rounded shapes, draw order, state-driven rendering, named constants versus magic numbers, the difference between data and presentation.

**Decisions:** Choose paddle dimensions and edge insets. Decide whether paddle position is stored as its center or its corner. Pick colors and glow treatments for each side.

**Done when:**

- The paddles and ball appear where the state says they should.
- Changing a state value in the console visibly moves or resizes the object on the next redraw.
- Sizes and positions are easy to adjust without hunting through the drawing code.

**Stretch:** Add a short ball trail or a center-circle emblem.

**Watch out:** Mixing state mutation into drawing code, confusing a paddle's center with its top edge, and scattering unexplained numbers throughout the file.

---

**Navigation:** **Previous:** [Phase 2 — Set up the canvas and draw the field](phase-02-canvas-field.md) · **Next:** [Phase 4 — Animate the ball and bounce off walls](phase-04-animation-and-walls.md)
