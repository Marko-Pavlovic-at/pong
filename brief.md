# Pong-ME — Learning Project Brief

A self-paced build plan for creating your own Pong-style game from scratch with plain HTML, CSS, and JavaScript.

This brief is a map, not a recipe. It deliberately contains **no code solutions**. You will make the design and implementation decisions, and the assistant will act as a coach and reviewer.

The project is split across four kinds of documents: this shared brief, one file per phase in `phases/`, a live tracker in `progress.md`, and a dated journal in `sessions.md`.

---

## 1. What you are building

A browser game with these **non-negotiable core features**:

- A human-controlled paddle and a computer-controlled paddle.
- A visible game field, ball, scoreboard, and start control.
- A **Start Game** button that begins play.
- The first player to reach **3 points** wins the current level.
- Winning a level advances you to the next one, up to **level 10**.
- Each level is harder than the last: the ball gets faster and the bot becomes more capable.
- Losing a level produces a clear game-over state with a way to try again.
- Winning level 10 produces a victory state.
- The game is playable with a keyboard and a mouse, and remains usable on a phone-sized screen.

You are encouraged to make your own visual theme, match flow, sound palette, and one personal gameplay twist. The finished game should feel like **your** version, not a clone of `pong-AI`.

### Out of scope for now

Online multiplayer, accounts, databases, 3D graphics, native mobile apps, complex physics engines, and large frameworks. Keep the project small enough to finish and understand.

---

## 2. Project constraints

- **Technology:** plain HTML, CSS, and JavaScript only. No frameworks, no game engines, no third-party libraries.
- **Rendering:** the playfield is drawn with the Canvas 2D API. Menus, HUD, and buttons are normal HTML elements.
- **Files:** start with `index.html`, `style.css`, and `game.js`. Split further only when it genuinely improves clarity.
- **Session size:** target one phase per 30–60 minute session. Some phases may take two sessions; that is expected.
- **Reference project:** `../pong-AI` is available, but it is a **last-resort fallback**, not a tutorial. See the fallback protocol below.
- **No copy-paste:** every line you keep should be a line you can explain.

---

## 3. How to use this brief

### Session workflow

1. Open the phase file for your current phase and read it in full before writing anything.
2. Open `progress.md` and mark the phase as **In progress** with the date.
3. Build the phase in small, testable increments. Refresh the browser often.
4. Use the phase's **Done when** checklist as your self-test.
5. Write a dated session entry in `sessions.md`: what you built, what worked, what is unfinished, and what you will do next.
6. Ask the assistant to review the phase. The assistant inspects the project, gives feedback, updates `progress.md`, and adds a review entry to `sessions.md` before you move on.

### The hints ladder

When you are stuck, work down this list before asking for help:

1. Re-read the phase goal and the definition of done.
2. Inspect the browser DevTools console and the actual game state.
3. Search the specific concept on MDN or another reference.
4. Explain the problem out loud as if teaching it to someone else.
5. Ask the assistant for a **hint or a question**, not a solution.
6. Only as a last resort, open `pong-AI` to study one small part.

### Fallback protocol for the reference project

If you open the reference code:

- Note it in `sessions.md` and say exactly what you looked at.
- Do not copy files, functions, or variable names wholesale.
- Close it, then rewrite the idea yourself without looking.
- Explain the result to the assistant before marking the phase reviewed.

The goal is a working mental model, not a working folder.

---

## 4. Milestones and phase files

| Milestone | Phases | Outcome |
|---|---|---|
| **A. Foundations** | 0–3 | A well-structured static game screen with a drawn field, paddles, and ball |
| **B. Playable core** | 4–8 | A moving ball, human control, collisions, a bot, and scoring |
| **C. Game structure** | 9–11 | Menus, levels, match rules, and a real difficulty curve |
| **D. Feel and robustness** | 12–16 | Stable physics, visual feedback, sound, mobile support, and testing |
| **E. Make it yours** | 17 | A personalized, documented, finished game |

Each phase file includes:

- **Goal** — why the phase exists.
- **Build** — the concrete result you should have at the end.
- **Concepts** — ideas and browser capabilities worth learning.
- **Decisions** — choices you should consciously make.
- **Done when** — observable acceptance criteria.
- **Stretch** — optional extra challenges.
- **Watch out** — common traps, without spoiling the solution.

### Phase files

Each phase below is a standalone file. Open the file for the phase you are working on; the shared rules in this brief still apply to every phase.

| Phase | Focus | Milestone |
|---|---|---|
| 0 | [Workspace and tools](phases/phase-00-setup.md) | A — Foundations |
| 1 | [Static game shell and scoreboard](phases/phase-01-static-shell.md) | A — Foundations |
| 2 | [Canvas setup and field drawing](phases/phase-02-canvas-field.md) | A — Foundations |
| 3 | [Paddles, ball, and game state](phases/phase-03-paddles-and-ball.md) | A — Foundations |
| 4 | [Animation loop and wall bounces](phases/phase-04-animation-and-walls.md) | B — Playable core |
| 5 | [Human paddle controls](phases/phase-05-human-control.md) | B — Playable core |
| 6 | [Paddle collision and angled returns](phases/phase-06-collision-and-returns.md) | B — Playable core |
| 7 | [Bot opponent](phases/phase-07-bot-opponent.md) | B — Playable core |
| 8 | [Scoring, serve, and reset](phases/phase-08-scoring-and-serve.md) | B — Playable core |
| 9 | [Match, levels, and state machine](phases/phase-09-match-and-levels.md) | C — Game structure |
| 10 | [Overlay screens and HUD flow](phases/phase-10-overlays-and-hud.md) | C — Game structure |
| 11 | [Difficulty curve for levels 1–10](phases/phase-11-difficulty-curve.md) | C — Game structure |
| 12 | [Stable physics at high speed](phases/phase-12-stable-physics.md) | D — Feel and robustness |
| 13 | [Visual feedback and game feel](phases/phase-13-game-feel.md) | D — Feel and robustness |
| 14 | [Sound and mute control](phases/phase-14-sound.md) | D — Feel and robustness |
| 15 | [Mobile, touch, and responsive layout](phases/phase-15-mobile-and-touch.md) | D — Feel and robustness |
| 16 | [Accessibility, resilience, testing](phases/phase-16-accessibility-and-testing.md) | D — Feel and robustness |
| 17 | [Personal twist, README, wrap-up](phases/phase-17-personalize-and-ship.md) | E — Make it yours |

---

## 5. Definition of done for the whole project

- [ ] Start screen with a working Start Game button
- [ ] Human paddle playable by keyboard and pointer
- [ ] Bot opponent that is beatable but capable
- [ ] Ball moves, bounces, and collides reliably at every level
- [ ] First to 3 points wins a level
- [ ] Ten levels with a clear difficulty increase
- [ ] Game over with retry, and victory after level 10
- [ ] Scores, serves, and levels reset correctly
- [ ] Pause, resume, blur, and visibility behavior are safe
- [ ] Readable HUD and overlays at desktop, tablet, and phone sizes
- [ ] Touch controls that do not fight page scrolling
- [ ] Sound with a working, persistent mute option
- [ ] Clean console through a full run
- [ ] `README.md`, a complete `progress.md`, and an up-to-date `sessions.md`
- [ ] At least one personal twist that makes the game yours

---

## 6. Ideas for your personal twist

Pick one, not all of them:

- A different visual era or sport: table tennis, squash, retro CRT, blueprint, paper sketch, neon nightclub, deep sea.
- A rule change: first-to-5, sudden death, shrinking paddles, a moving goal, power-ups, a central obstacle.
- A bot personality: nervous, arrogant, adaptive, deliberately inconsistent, or one that learns your favorite angle.
- A progression change: three lives across the ten levels, boss levels, or a choice between two difficulty paths.
- A presentation change: a commentary feed, crowd noise, an animated crowd, or a replay of the winning point.

Whatever you choose, keep the core loop intact and playable.

---

## 7. Self-assessment rubric

Score yourself honestly at the end of each milestone.

| Area | 1 — Needs work | 3 — Solid | 5 — Strong |
|---|---|---|---|
| **Functionality** | Core loop breaks often | Full run works with minor issues | Full loop is robust across states and devices |
| **Code clarity** | One long file, unclear names | Clear sections and named state | Small, testable units and obvious data flow |
| **Learning** | Copied without understanding | Can explain most decisions | Can explain, critique, and adapt every system |
| **Polish** | Barely usable | Clear feedback and coherent style | Distinctive and satisfying without harming clarity |
| **Originality** | Direct clone | Own visuals and some tuning | Own identity, rules, or meaningful twist |

An honest 3 across the board is a finished learning project. Chase 5s only after the 3s are stable.

---

## 8. The assistant's coaching contract

During this project, the assistant will:

- Answer concept questions with explanations, analogies, and questions.
- Review your code for clarity, correctness, and learning opportunities.
- Point out symptoms and likely causes without immediately writing the fix.
- Give small hints when you are stuck, escalating only if you ask for more.
- Refuse to hand you complete solutions, in line with this brief.
- Update `progress.md` after each review and add a review entry to `sessions.md`, so the next session starts with accurate context.
- Keep the plan flexible: if a phase is too large or too small, say so and we will adjust it.

When you are ready for a review, say: **“Review phase [number].”** The assistant will inspect the project, test what it can, leave feedback, and record the outcome in `progress.md` and `sessions.md`.

---

## 9. Start here

1. Read [Phase 0](phases/phase-00-setup.md) and [Phase 1](phases/phase-01-static-shell.md) once.
2. Set up the three files.
3. Fill in the first session in `sessions.md`.
4. Build Phase 0, then ask for a review. Do not skip the setup review; it establishes the testing and feedback habits the rest of the project depends on.
