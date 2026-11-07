# Pong-ME — Session Log

This file is the dated journal for the project. It records what you actually did, in the order you did it, so a later session can resume without guessing.

- **Project brief:** [brief.md](brief.md)
- **Phase files:** [phases/](phases/)
- **Progress tracker:** [progress.md](progress.md)
- **Reference (fallback only):** `../pong-AI`
- **Started:** 2026-11-05
- **Next session:** Session 1

New entries go at the top. Keep them short and concrete. It is fine to record a messy session; honesty is more useful than a perfect write-up.

---

## How to use this log

1. At the start of a session, add a dated heading with the phase and the goal you intend to work on.
2. While working, jot down decisions, surprises, and blockers as they happen.
3. At the end, fill in what was built, what worked, what is unfinished, and the next step.
4. When a phase meets its "Done when" criteria, set it to **Ready for review** in `progress.md` and ask the assistant for a review.
5. After a review, the assistant adds a review entry below and updates `progress.md`.
6. Never delete an old entry to make the log look cleaner. Add a correction or follow-up instead.

---

## Session log

### Session 0 — 2026-11-05 — Project setup

- **Phase:** None — planning
- **What happened:** Created the brief, the per-phase files, the progress tracker, and this session log. Agreed on plain HTML/CSS/JS, small 30–60 minute phases, and using `../pong-AI` only as a fallback.
- **What worked:** Scope, technology, document structure, and review process are defined.
- **Unfinished / blockers:** No game files exist yet.
- **Next step:** Start Phase 0 — create the three project files and confirm a clean browser console.

---

## Session entry template

Copy this structure into the log when adding a new entry.

> ### Session N — YYYY-MM-DD — Phase N title
>
> - **Phase:** Phase N — title
> - **Goal for this session:** what you intend to finish
> - **What I built:** the concrete change or feature
> - **What worked:** what behaved as intended
> - **What I learned:** the concept that became clearer
> - **Decisions made:** anything worth remembering
> - **Unfinished / blockers:** what is left or what stopped progress
> - **Next step:** the first action for the next session

---

## Review entry template

Use this structure when recording the outcome of a phase review. The assistant fills this in and updates `progress.md`.

> ### Review — YYYY-MM-DD — Phase N title
>
> - **Status after review:** Reviewed / Needs work
> - **Observed:** the current behavior and implementation state
> - **Working well:** strengths worth keeping
> - **Must fix:** items required to meet the phase's definition of done
> - **Concepts demonstrated:** what the work proves was learned
> - **Concepts to revisit:** what still needs practice
> - **Question asked:** the user's explanation of a key decision
> - **Next focus:** the next phase or the smallest missing piece

---

## Logging tips

- Name the file or screen you changed, not just the concept.
- Record the exact error message or symptom when something breaks.
- Distinguish "finished" from "works for now"; both are useful, but they mean different things.
- If you consult the reference project, write down what you looked at and what you rebuilt yourself.
- End every entry with one next step, even if the session went badly.
