[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 5 — Control the human paddle

**Milestone B — Playable core**

**Goal:** Make the player's paddle feel direct and reliable with mouse, touch, and keyboard.

**Build:**

- Pointer control that maps the cursor or finger position to the paddle's vertical position.
- Keyboard control with held keys, not repeated single presses.
- Clamping so the paddle never leaves the field.
- A deliberate follow behavior: direct, smoothed, or speed-limited.
- Input that still works after the window is resized.

**Concepts:** pointer events, keyboard events and held-key state, client coordinates versus canvas coordinates, element bounding rectangles, coordinate conversion, clamping, easing and smoothing, event-driven input versus per-frame input, touch-action and scroll prevention.

**Decisions:** Should the paddle teleport to the pointer or chase it? How fast should keyboard movement be? Should the two control styles coexist, and which takes priority?

**Done when:**

- Mouse, touch, and keyboard all move the paddle predictably.
- The paddle stops exactly at both boundaries.
- Moving the mouse outside the canvas does not break control.
- The page does not scroll while dragging inside the field.

**Stretch:** Add a subtle paddle tilt or glow that reacts to movement.

**Watch out:** Using page coordinates directly without converting them, listening only to click instead of movement, key-repeat delays, and touch gestures scrolling the page.

---

**Navigation:** **Previous:** [Phase 4 — Animate the ball and bounce off walls](phase-04-animation-and-walls.md) · **Next:** [Phase 6 — Collide with the paddle and aim returns](phase-06-collision-and-returns.md)
