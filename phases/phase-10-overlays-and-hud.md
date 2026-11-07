[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 10 — Build the overlay and HUD experience

**Milestone C — Game structure**

**Goal:** Make the game's non-playfield UI feel like one coherent product.

**Build:**

- Readable overlay screens for start, pause, level cleared, game over, and victory.
- Contextual information on each screen: rules, score, level, and the next action.
- Buttons that always do what they say.
- Keyboard shortcuts for the primary action, plus pause and resume.
- Pause behavior when the window loses focus or the tab becomes hidden.
- Focus that lands somewhere sensible when a screen opens.

**Concepts:** HTML overlays over a canvas, conditional rendering, safe text versus HTML insertion, focus management, keyboard activation, pause semantics, the visibility API, window blur, button states, accessible dialog patterns.

**Decisions:** Is the overlay a full-screen layer or limited to the playfield? Should the game auto-pause on blur? How prominent is each action?

**Done when:**

- Every screen is readable at desktop and phone widths.
- Space or Enter activates the expected primary action.
- Pause stops the game, and resume continues it cleanly.
- No menu allows the ball to keep moving behind it.
- Focus and hover states are visible.

**Stretch:** Add a short countdown before the next level.

**Watch out:** Overlays clipped by their containers, accidental double actions, focus disappearing, and showing the wrong message for the current score.

---

**Navigation:** **Previous:** [Phase 9 — Build the match and level structure](phase-09-match-and-levels.md) · **Next:** [Phase 11 — Design the difficulty curve and the ten levels](phase-11-difficulty-curve.md)
