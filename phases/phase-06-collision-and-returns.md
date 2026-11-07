[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 6 — Collide with the paddle and aim returns

**Milestone B — Playable core**

**Goal:** Turn paddle contact into controllable, satisfying returns.

**Build:**

- Detection of when the ball reaches the human paddle and overlaps it.
- A return that sends the ball back toward the bot, with the angle influenced by where the ball struck the paddle.
- Protection against the ball sticking inside the paddle or triggering the same hit repeatedly.
- A safe response if the ball is moving unusually fast.

**Concepts:** circle-versus-rectangle collision, axis-aligned bounding boxes, previous and current positions, hit offset, angle mapping, reflection, velocity normalization, collision ordering, tunneling, speed caps.

**Decisions:** How wide should the return-angle range be? Should the paddle's own motion add spin? Should each hit speed the ball up, and by how much?

**Done when:**

- Center hits return the ball roughly straight; edge hits send it at sharper angles.
- The ball never gets trapped inside the paddle.
- A fast ball does not pass straight through under normal play.
- Returns feel intentional rather than random.

**Stretch:** Add paddle-motion spin and a small impact effect.

**Watch out:** Reflecting only one axis when two are involved, repositioning the ball without reversing its direction, and checking collisions after the ball has already moved too far.

---

**Navigation:** **Previous:** [Phase 5 — Control the human paddle](phase-05-human-control.md) · **Next:** [Phase 7 — Create a bot opponent](phase-07-bot-opponent.md)
