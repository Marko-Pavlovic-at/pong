[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 14 — Add sound with user control

**Milestone D — Feel and robustness**

**Goal:** Reinforce events with audio that is pleasant, optional, and technically well-behaved.

**Build:**

- Short sounds for paddle hits, wall bounces, points, level win, and game over or victory.
- A mute control that is easy to find and works immediately.
- A remembered sound preference between visits.
- Audio that only starts after a user interaction.
- A graceful experience when audio is unavailable.

**Concepts:** Web Audio API versus HTML audio elements, oscillators and gain envelopes, audio context lifecycle, autoplay restrictions, user gestures, event-driven sound, localStorage with safe fallbacks, volume and sensory consideration.

**Decisions:** Should sounds be synthesized or loaded from files? How loud is too loud? Should hit pitch vary with speed? Should muting be global and persistent?

**Done when:**

- Each major event has an audible cue.
- Muting stops sound and updates the visible control.
- The preference survives a refresh.
- No console errors appear in a browser that blocks audio.

**Stretch:** Vary the hit pitch with ball speed, or add a subtle ambience toggle.

**Watch out:** Creating an audio context before a gesture, stacking loud overlapping tones, and forgetting to persist or reflect the mute state.

---

**Navigation:** **Previous:** [Phase 13 — Add feedback and game feel](phase-13-game-feel.md) · **Next:** [Phase 15 — Make it work on phones and tablets](phase-15-mobile-and-touch.md)
