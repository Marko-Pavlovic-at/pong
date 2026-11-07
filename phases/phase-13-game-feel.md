[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 13 — Add feedback and game feel

**Milestone D — Feel and robustness**

**Goal:** Make events legible and satisfying without turning the screen into noise.

**Build:**

- A ball trail that communicates speed and direction.
- Impact particles or sparks at paddles and walls.
- A restrained screen shake on important hits and points.
- Goal flashes or color washes that identify who scored.
- A serve indicator showing where the ball will launch.
- A score animation in the HUD.
- Respect for reduced-motion preferences.

**Concepts:** transient effect systems, arrays of short-lived objects, lifespan and cleanup, alpha and compositing, easing, screen shake, performance budgets, visual hierarchy, prefers-reduced-motion, accessibility of motion.

**Decisions:** Which events deserve feedback? How long should effects live? Should the shake be global or local? What is your visual signature?

**Done when:**

- A player can tell what happened without reading text.
- Effects clean themselves up and do not slow the game over time.
- The scene remains readable during the fastest rallies.
- Reduced-motion users get a calmer experience.

**Stretch:** Add a victory confetti burst or an animated ambient background.

**Watch out:** Unbounded particle arrays, effects that obscure the ball, and motion that looks impressive for five seconds and exhausting after five minutes.

---

**Navigation:** **Previous:** [Phase 12 — Make the physics stable at high speed](phase-12-stable-physics.md) · **Next:** [Phase 14 — Add sound with user control](phase-14-sound.md)
