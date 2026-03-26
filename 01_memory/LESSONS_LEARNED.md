# Lessons Learned

Every mistake, surprise, and shortcut discovered. Read this before starting a new project.

---

## Lesson 001 — Reserved JavaScript Variable Names (2026-03-26)

**Project:** Amazon BPMN
**Problem:** Named a helper function `top()` in JavaScript. The browser uses `window.top` as a reserved global, causing: `Identifier 'top' has already been declared`.
**Fix:** Renamed to `nodeTop()`. Checked the entire file for other reserved names.
**Rule:** Never name JS functions or variables: `top`, `name`, `location`, `parent`, `self`, `frames`, `screen`, `history`, `event`.

---

## Lesson 002 — Auto-Fit Zoom Needs Dynamic Calculation (2026-03-26)

**Project:** Amazon BPMN
**Problem:** Used a fixed `scale = 0.72` which cut off the diagram on some screens.
**Fix:** Replaced with `fitToScreen()` that calculates `scale = Math.min(availW / CANVAS_W, availH / CANVAS_H)` at load and on resize.
**Rule:** Never hardcode zoom/scale values. Always calculate from viewport dimensions.

---

## Lesson 003 — Node Size Affects Everything Downstream (2026-03-26)

**Project:** Amazon BPMN
**Problem:** Reducing node width required updating all positions, canvas size, arrow offsets, gateway offsets, and curved arrow waypoints.
**Fix:** Ask Claude to "recalculate all positions, canvas dimensions, and arrow offsets proportionally."
**Rule:** When changing node size, always explicitly ask for proportional recalculation of everything.

---

## Lesson 004 — Context First, Always (2026-03-26)

**Project:** Amazon BPMN
**Insight:** The richer the context in prompt_01, the less refinement needed later.
**Rule:** Spend at least 10 minutes on Perplexity research before writing the master prompt.

---

## Add new lessons below this line

## Lesson 005 — [Title] (YYYY-MM-DD)

**Project:**
**Problem:**
**Fix:**
**Rule:**
