[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 4 — Animate the ball and bounce off walls

**Milestone B — Playable core**

**Goal:** Introduce a real game loop and frame-rate-independent motion.

**Build:**

- A continuous animation loop using the browser's frame callback.
- An update step and a separate render step.
- A ball with a velocity that moves smoothly and bounces off the top and bottom boundaries.
- Motion that behaves consistently on fast and slow machines.
- A clean way to stop or pause the loop later.

**Concepts:** requestAnimationFrame, timestamps, milliseconds versus seconds, delta time, velocity vectors, boundary collision, reflection, clamping, separating simulation from rendering, frame-rate independence.

**Decisions:** Choose your speed units and starting direction. Decide whether the ball should reflect symmetrically or gain a little energy on wall hits.

**Done when:**

- The ball moves smoothly and stays inside the field.
- The motion speed is not tied to the monitor's refresh rate.
- Returning to the tab after a pause does not teleport the ball wildly.
- The update logic can run without drawing, and drawing can happen without changing state.

**Stretch:** Make wall bounces produce a small visual effect.

**Watch out:** Using raw frame counts instead of elapsed time, huge delta values after the tab was inactive, and updating positions inside the render routine.

---

**Navigation:** **Previous:** [Phase 3 — Give the game state a shape: paddles and ball](phase-03-paddles-and-ball.md) · **Next:** [Phase 5 — Control the human paddle](phase-05-human-control.md)
