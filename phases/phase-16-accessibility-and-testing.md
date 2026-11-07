[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 16 — Accessibility, resilience, and testing

**Milestone D — Feel and robustness**

**Goal:** Turn a working game into a dependable one.

**Build:**

- Full keyboard play and visible focus states.
- Pause on window blur and tab hide.
- A reduced-motion path.
- A short browser test matrix and a written bug list with fixes.
- Edge-case tests: pause during a serve, score on the final point, retry after game over, resize mid-rally, mute state after reload.
- A clean console on every screen.

**Concepts:** accessibility tree, focus order, keyboard operability, ARIA only when necessary, color contrast, reduced motion, `visibilitychange` and blur, QA checklists, reproducible bug reports, browser compatibility, performance inspection.

**Decisions:** Which accessibility support is essential? Which browsers are your minimum bar? How will you track bugs?

**Done when:**

- The game can be played without a mouse.
- Pausing and resuming in every state is safe.
- No known bug can trap the player without an escape.
- The console is clean during a full run in at least two browsers.
- Your test notes list what you tried and what remains risky.

**Stretch:** Announce scores to assistive technology without making the game noisy.

**Watch out:** Adding ARIA that duplicates native button behavior, testing only one browser, and fixing bugs without recording how to reproduce them.

---

**Navigation:** **Previous:** [Phase 15 — Make it work on phones and tablets](phase-15-mobile-and-touch.md) · **Next:** [Phase 17 — Make it yours and wrap up](phase-17-personalize-and-ship.md)
