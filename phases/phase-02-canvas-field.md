[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 2 — Set up the canvas and draw the field

**Milestone A — Foundations**

**Goal:** Learn how the canvas coordinate system, sizing, and drawing model work.

**Build:**

- A canvas that occupies the game area and keeps a consistent internal aspect ratio.
- A single drawing routine that paints the background, boundaries, center line, and any field markings.
- Crisp visuals on high-density screens.
- A clear separation between the canvas's internal resolution and its displayed size.

**Concepts:** canvas coordinate space versus CSS pixels, width and height attributes, the 2D drawing context, rectangles, lines, circles, paths, fill and stroke styles, shadows and glow, aspect ratio, device pixel ratio, redrawing and clearing.

**Decisions:** Choose an internal resolution (for example, a wide landscape ratio). Decide whether the canvas should scale with the window or sit at a fixed maximum size. Choose a field style that supports your theme.

**Done when:**

- The field is drawn deliberately, not accidentally.
- Resizing the window does not distort or blur it badly.
- You can explain the difference between the canvas's pixel size and its CSS size.
- The field can be redrawn from scratch without leftover artifacts.

**Stretch:** Add a subtle grid, vignette, or animated ambient glow.

**Watch out:** Setting only CSS size or only the canvas attributes, blurry rendering on retina displays, and forgetting that most canvas scenes must be fully redrawn each frame.

---

**Navigation:** **Previous:** [Phase 1 — Build the static game shell](phase-01-static-shell.md) · **Next:** [Phase 3 — Give the game state a shape: paddles and ball](phase-03-paddles-and-ball.md)
