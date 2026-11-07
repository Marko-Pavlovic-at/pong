[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 9 — Build the match and level structure

**Milestone C — Game structure**

**Goal:** Turn individual rallies into a complete game with menus, levels, and endings.

**Build:**

- A start screen and a working **Start Game** button.
- A clear distinction between menu, playing, paused, level-cleared, game-over, and victory states.
- The first-to-3 rule for each level.
- Level progression from 1 to 10.
- A game-over state when the bot wins, with a retry option.
- A victory state after winning level 10.
- Reset rules so scores and positions never leak between levels.

**Concepts:** finite state machines, explicit modes versus implicit flags, transitions, guards, score resets, level progression, button-triggered actions, keeping simulation stopped in non-playing states.

**Decisions:** Does losing reset the whole run or only the current level? Does the next level start automatically or wait for a button? How much information should each screen show?

**Done when:**

- You can start a game, win a level, and reach level 2.
- You can win all the way to level 10 and see a victory screen.
- You can lose a level and recover without reloading the page.
- Physics does not continue running while any menu is open.
- Scores always reset to zero for a new level.

**Stretch:** Add a short post-level summary with the score and the next difficulty.

**Watch out:** Multiple states being true at once, event handlers firing twice, and scores carrying over because reset logic lives in the wrong place.

---

**Navigation:** **Previous:** [Phase 8 — Score points and reset the rally](phase-08-scoring-and-serve.md) · **Next:** [Phase 10 — Build the overlay and HUD experience](phase-10-overlays-and-hud.md)
