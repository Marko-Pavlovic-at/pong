[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 15 — Make it work on phones and tablets

**Milestone D — Feel and robustness**

**Goal:** Deliver a genuinely playable mobile experience, not a shrunken desktop page.

**Build:**

- Touch dragging that controls the paddle without scrolling the page.
- Layout adjustments that keep the HUD, field, and controls usable at narrow widths.
- Overlays that fit or scroll instead of being clipped.
- Correct pointer mapping after the canvas changes size.
- A strategy for very short viewports and landscape orientation.

**Concepts:** viewport meta settings, responsive units, aspect ratio, media queries, pointer events, touch-action, fixed-position overlays and containment, device pixel ratio, tap-target sizing, orientation changes.

**Decisions:** Do overlays take over the viewport on phones? What is the minimum playable field size? Should you prompt the player to rotate the device?

**Done when:**

- You can start, play, win, lose, and resume on a phone-sized screen.
- Buttons are reachable and finger-sized.
- Dragging does not scroll or zoom the page.
- The field and overlays remain aligned after rotation.

**Stretch:** Add a fullscreen control or a portrait-mode orientation hint.

**Watch out:** Fixed overlays trapped by an ancestor, tiny tap targets, and desktop-only hover assumptions.

---

**Navigation:** **Previous:** [Phase 14 — Add sound with user control](phase-14-sound.md) · **Next:** [Phase 16 — Accessibility, resilience, and testing](phase-16-accessibility-and-testing.md)
