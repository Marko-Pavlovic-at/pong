[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 8 — Score points and reset the rally

**Milestone B — Playable core**

**Goal:** Close the loop of a point: detect a miss, update the score, and serve again.

**Build:**

- Detection of the ball leaving the field on either side.
- Exactly one point awarded per miss.
- A visible score update in the HUD.
- A serve/reset sequence with a short delay, a centered ball, and a clear initial direction.
- Feedback that a point happened.

**Concepts:** out-of-bounds detection, one-shot events, scoring rules, state reset, one-shot timers using delta time, serve direction, DOM updates, edge cases and guard clauses.

**Decisions:** Who receives the serve after a point? How long is the pause before the next serve? Should the ball launch automatically or wait for input? How much visual feedback is enough?

**Done when:**

- The correct player gains a point when the ball exits each side.
- A single miss cannot award multiple points.
- The ball, scores, and paddle positions reset consistently.
- The HUD never drifts from the internal score.

**Stretch:** Add a three-second serve countdown or an aim indicator.

**Watch out:** Awarding a point on multiple frames, resetting position but forgetting velocity, and letting the HUD update in more than one conflicting place.

---

**Navigation:** **Previous:** [Phase 7 — Create a bot opponent](phase-07-bot-opponent.md) · **Next:** [Phase 9 — Build the match and level structure](phase-09-match-and-levels.md)
