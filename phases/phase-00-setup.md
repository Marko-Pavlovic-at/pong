[← Project brief](../brief.md) · [All phases](../brief.md#4-milestones-and-phase-files) · [Progress tracker](../progress.md) · [Session log](../sessions.md)

# Phase 0 — Set up a workspace you can trust

**Milestone A — Foundations**

**Goal:** Start with a clean, connected project and know how to inspect it when things go wrong.

**Build:**

- A `pong-ME` folder containing `index.html`, `style.css`, and `game.js`, all linked correctly.
- A page that displays at least a heading and loads without errors.
- A working habit of checking the browser console.
- Optional but recommended: a Git repository with one initial commit.

**Concepts:** relative file paths, how the browser loads CSS and JavaScript, script placement and loading order, browser DevTools (console, elements, network), local development versus opening a file directly, version control basics.

**Decisions:** Will you open the files directly or use a local server? Which browser will be your main test browser? Where will you keep notes?

**Done when:**

- The page loads and the heading is visible.
- A deliberate edit to the heading appears after refresh.
- The console shows no errors.
- You can open and navigate DevTools without help.

**Stretch:** Add a favicon, or test the page through a local development server instead of opening the file directly.

**Watch out:** wrong relative paths, a script running before the page elements exist, stale cached files, and testing only by assuming the page worked.

---

**Navigation:** **Previous:** — · **Next:** [Phase 1 — Build the static game shell](phase-01-static-shell.md)
