[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 12 — Make the physics stable at high speed

**Milestone D — Feel and robustness**

**Goal:** Ensure the game stays correct when the ball is at its fastest.

**Build:**

- A timestep strategy that prevents fast balls from tunneling through paddles.
- Explicit maximum ball speed and a safe acceleration policy.
- Correct collision ordering when a wall and a paddle are hit close together.
- Reliable pause and resume without accumulated time causing a jump.
- A ball trajectory that remains predictable enough to be fair.

**Concepts:** fixed timesteps, accumulators, sub-stepping, variable versus fixed delta, tunneling, continuous versus discrete collision, velocity caps, max frame catch-up, determinism, numerical stability.

**Decisions:** What simulation step size do you need? How much catch-up is acceptable after a slow frame? Do you advance the ball in several smaller moves? Where do speed limits apply?

**Done when:**

- At maximum level, the ball never passes through the paddle.
- A long pause does not cause a burst of catch-up movement.
- Collision results are consistent at different frame rates.
- The game remains responsive and does not spiral into slow motion.

**Stretch:** Add swept collision or predictive collision for very small step counts.

**Watch out:** Letting the accumulator grow forever, resetting time incorrectly after pause, and capping speed only at serve time.

---

**Navigation:** **Previous:** [Phase 11 — Design the difficulty curve and the ten levels](phase-11-difficulty-curve.md) · **Next:** [Phase 13 — Add feedback and game feel](phase-13-game-feel.md)
