[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 7 — Create a bot opponent

**Milestone B — Playable core**

**Goal:** Build an opponent that is competent, tunable, and clearly beatable.

**Build:**

- A bot paddle that tracks the ball and returns it.
- Tunable behavior: maximum speed, reaction delay, prediction skill, and aiming error.
- The ability for the bot to miss when outplayed.
- No frame-by-frame jitter or superhuman instant reactions.

**Concepts:** target tracking, prediction versus reaction, maximum speed and time-to-target, reaction timers, bounded randomness, aiming error, wall-bounce prediction, difficulty parameters, simple AI design.

**Decisions:** How does the bot decide where to go? How often may it revise its target? Should it predict wall bounces perfectly or only partly? How should difficulty change its behavior later?

**Done when:**

- The bot can sustain a rally.
- A well-aimed shot can beat it.
- Its paddle movement looks smooth rather than twitchy.
- Changing one bot parameter produces a noticeable, understandable difference.

**Stretch:** Make the bot sometimes commit early to a guess, leaving it vulnerable to angled shots.

**Watch out:** Recomputing an exact target every frame, using unbounded randomness that causes jitter, and creating a bot that is technically beatable but effectively perfect.

---

**Navigation:** **Previous:** [Phase 6 — Collide with the paddle and aim returns](phase-06-collision-and-returns.md) · **Next:** [Phase 8 — Score points and reset the rally](phase-08-scoring-and-serve.md)
