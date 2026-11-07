[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 11 — Design the difficulty curve and the ten levels

**Milestone C — Game structure**

**Goal:** Make levels 1 through 10 feel meaningfully different, fair, and finishable.

**Build:**

- A documented difficulty plan for all ten levels.
- A parameter table for ball speed, ball acceleration, bot speed, bot reaction, bot accuracy, and prediction.
- A clear ramp: level 1 should teach, level 10 should demand focus.
- Playtest notes showing what changed and why.
- Protection against endless rallies and unwinnable configurations.

**Concepts:** parameterization, difficulty curves and stepped difficulty, linear versus exponential scaling, speed caps, randomness distributions, fairness, playtesting, collecting observations, tuning by iteration, separating tuning data from logic.

**Decisions:** Which values change per level? How steep is the ramp? Should difficulty be continuous or jump between tiers? What makes level 10 hard without making it unfair?

**Done when:**

- Each level is demonstrably harder than the previous one.
- Level 1 is approachable for a new player.
- Level 10 is challenging but has been won at least once.
- No level produces a rally that never ends under normal play.
- The tuning values live in a place that is easy to adjust.

**Stretch:** Add a hidden assist mode, or an adaptive bot that eases off after repeated losses.

**Watch out:** Increasing only ball speed, giving the bot perfect accuracy, using randomness as a substitute for design, and balancing against only one lucky match.

---

**Navigation:** **Previous:** [Phase 10 — Build the overlay and HUD experience](phase-10-overlays-and-hud.md) · **Next:** [Phase 12 — Make the physics stable at high speed](phase-12-stable-physics.md)
