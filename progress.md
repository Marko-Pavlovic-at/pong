# Pong-ME — Progress Tracker

This file is the live state of the project. It tracks where you are, what is blocked, and what comes next. The detailed, dated story of each session lives in `sessions.md`.

- **Project:** Pong-ME — a personal Pong-style game
- **Brief:** [brief.md](brief.md)
- **Phase files:** [phases/](phases/)
- **Session log:** [sessions.md](sessions.md)
- **Reference (fallback only):** `../pong-AI`
- **Stack:** plain HTML, CSS, and JavaScript
- **Session size:** 30–60 minutes
- **Started:** 2026-11-05
- **Last updated:** 2026-11-05

---

## Current snapshot

| Field | Value |
|---|---|
| **Current phase** | Phase 0 — Set up a workspace you can trust |
| **Phase status** | Not started |
| **Completed phases** | 0 of 18 |
| **Next action** | Create `index.html`, `style.css`, and `game.js`; link them; confirm a clean console |
| **Current blocker** | None |
| **Last review** | None yet |

> Keep this table current. It is the first thing to read at the start of a session.

---

## Phase tracker

Status values: **Not started**, **In progress**, **Ready for review**, **Needs work**, **Reviewed**.

| Phase | Focus | Status | Started | Reviewed | Notes |
|---|---|---|---|---|---|
| 0 | [Workspace and tools](phases/phase-00-setup.md) | Not started | — | — | — |
| 1 | [Static game shell and scoreboard](phases/phase-01-static-shell.md) | Not started | — | — | — |
| 2 | [Canvas setup and field drawing](phases/phase-02-canvas-field.md) | Not started | — | — | — |
| 3 | [Paddles, ball, and game state](phases/phase-03-paddles-and-ball.md) | Not started | — | — | — |
| 4 | [Animation loop and wall bounces](phases/phase-04-animation-and-walls.md) | Not started | — | — | — |
| 5 | [Human paddle controls](phases/phase-05-human-control.md) | Not started | — | — | — |
| 6 | [Paddle collision and angled returns](phases/phase-06-collision-and-returns.md) | Not started | — | — | — |
| 7 | [Bot opponent](phases/phase-07-bot-opponent.md) | Not started | — | — | — |
| 8 | [Scoring, serve, and reset](phases/phase-08-scoring-and-serve.md) | Not started | — | — | — |
| 9 | [Match, levels, and state machine](phases/phase-09-match-and-levels.md) | Not started | — | — | — |
| 10 | [Overlay screens and HUD flow](phases/phase-10-overlays-and-hud.md) | Not started | — | — | — |
| 11 | [Difficulty curve for levels 1–10](phases/phase-11-difficulty-curve.md) | Not started | — | — | — |
| 12 | [Stable physics at high speed](phases/phase-12-stable-physics.md) | Not started | — | — | — |
| 13 | [Visual feedback and game feel](phases/phase-13-game-feel.md) | Not started | — | — | — |
| 14 | [Sound and mute control](phases/phase-14-sound.md) | Not started | — | — | — |
| 15 | [Mobile, touch, and responsive layout](phases/phase-15-mobile-and-touch.md) | Not started | — | — | — |
| 16 | [Accessibility, resilience, testing](phases/phase-16-accessibility-and-testing.md) | Not started | — | — | — |
| 17 | [Personal twist, README, wrap-up](phases/phase-17-personalize-and-ship.md) | Not started | — | — | — |

---

## Decisions log

Record choices that would be expensive to rediscover later. Add a row whenever you make a significant decision.

| Date | Area | Decision | Reason |
|---|---|---|---|
| 2026-11-05 | Stack | Plain HTML, CSS, and JavaScript only | Keep the learning focused and the project dependency-free |
| 2026-11-05 | Phases | Small sessions of 30–60 minutes | Match the preferred learning pace |
| 2026-11-05 | Reference | Use `pong-AI` only as a last resort | Protect the learning value of building from scratch |
| 2026-11-05 | Coaching | No full code solutions; hints and reviews only | Learn through decisions, not transcription |

---

## Open questions and blockers

Use this section for anything that is genuinely unresolved. Remove items once answered.

- None yet.

---

## Concept confidence

Update the confidence score from 1 to 5 after each phase review. Use the notes column for evidence: what you built, explained, or debugged.

| Concept | Confidence (1–5) | Evidence or notes |
|---|---|---|
| Page structure and semantic HTML | — | — |
| CSS layout, spacing, and responsive rules | — | — |
| Canvas coordinate space and drawing | — | — |
| Animation loop and delta time | — | — |
| Pointer and keyboard input | — | — |
| Collision detection and reflection | — | — |
| Game state and state transitions | — | — |
| Bot behavior and difficulty tuning | — | — |
| DOM overlays and HUD updates | — | — |
| Audio and user preferences | — | — |
| Mobile and touch behavior | — | — |
| Testing, debugging, and accessibility | — | — |

A score of 1–2 means "can recognise it"; 3 means "can build it with references"; 4–5 means "can explain and adapt it confidently." Honest scores help tailor future hints.

---

## How to update this file

### After each work session

1. Set the phase status to **In progress** (or keep it if already open).
2. Write the detailed, dated entry in `sessions.md`.
3. Update any important decision in the decisions log here.
4. Add blockers or open questions where they belong.
5. Update the current snapshot and next action.
6. When the phase meets its "Done when" criteria, set it to **Ready for review**.

### After each review

The assistant updates:

- The phase status and review date.
- The current snapshot and next action.
- A review entry in `sessions.md`.
- Concept confidence scores where evidence exists.
- Decisions and blockers.

If a phase needs more work, its status becomes **Needs work**, and the next action names the smallest missing piece.

---

## Review protocol for the assistant

When the user asks for a phase review, follow this sequence.

1. **Read context.** Open the relevant phase file in `phases/`, the current status in this file, and the latest entries in `sessions.md`.
2. **Inspect the workspace.** Look at all project files, not just the most recently edited one.
3. **Exercise the project.** If possible, open it in a browser, check the console, and test the phase's key interaction. If browser access is unavailable, ask the user for the observed behavior.
4. **Check the criteria.** Compare the implementation against the phase's "Done when" list and the overall project constraints.
5. **Give feedback in this order:**
   - What works and why it matters.
   - What must be fixed before moving on.
   - The concepts the implementation demonstrates or misses.
   - One or two stretch ideas, only if the core is solid.
6. **Ask the user to explain one decision.** This verifies understanding and catches accidental copy-paste.
7. **Update this file:**
   - Phase status, started/reviewed dates, and tracker notes.
   - Current snapshot and next action.
   - A review entry in `sessions.md`.
   - Concept confidence when justified.
   - Decisions, open questions, and blockers.
8. **Do not provide a complete solution.** Give symptoms, questions, and the smallest useful hint. If the user is deeply stuck, offer a conceptual explanation or a debugging strategy, not finished code.
9. **Protect the learning plan.** If a phase is too large, propose splitting it; if too small, merge it with a neighbour. Record the change in the decisions log.

### Review feedback format

Use this structure, adapted as needed:

- **Observed:** what the project currently does.
- **Working well:** the strongest part of the phase.
- **Must fix:** only the issues that block the phase's definition of done.
- **Concepts to revisit:** one to three specific ideas.
- **Stretch (optional):** one challenge worth doing after the fix.
- **Question for the user:** one decision to explain in their own words.
- **Next step:** the single most valuable thing to do next.

---

## Project rules reminder

- One phase at a time; avoid jumping ahead because a later phase looks more interesting.
- Refresh and test after every meaningful change.
- No code is copied from the reference project without recording it and rebuilding it from understanding.
- Ask for hints before asking for solutions.
- If a session goes badly, record it honestly. A clear blocker is more useful than a vague "it broke."
- Keep the core requirements working as the project grows; polish never excuses a broken loop.
