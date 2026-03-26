# Chain Command: Full Pipeline

Run this for every new project from start to finish.

---

## BEFORE YOU START
Copy `07_templates_master/NEW_PROJECT_KICKOFF.md`, fill it in (5 min), save as `06_projects/{name}/BRIEF.md`.

---

## STEP 1 — Context Collection (Agent 1)
**Tool:** Perplexity | **Time:** ~10 min

1. Open `03_prompts/templates/PROMPT_context_collector.md`
2. Fill in your topic and run in Perplexity
3. Save output as `03_prompts/projects/{name}/prompt_01_context.md`

Done when: You have all steps, roles, decisions, and exceptions documented.

---

## STEP 2 — Prompt Architecture (Agent 2)
**Tool:** ChatGPT | **Time:** ~10 min

1. Open `03_prompts/templates/PROMPT_architect_master.md`
2. Paste your `prompt_01_context.md` at the bottom
3. Run in ChatGPT
4. Save JSON output as `03_prompts/projects/{name}/prompt_02_json_master.md`

Done when: You have a clean JSON-structured master prompt.

---

## STEP 3 — Build (Agent 3)
**Tool:** Claude | **Time:** ~5 min (Claude builds it)

1. Open `03_prompts/templates/PROMPT_builder_html.md`
2. Paste your `prompt_02_json_master.md` at the bottom
3. Run in Claude
4. Save output as `06_projects/{name}/ASSETS/output_v1.html`
5. Open in browser and test

Done when: File opens and shows the output correctly.

---

## STEP 4 — Refine (Agent 4)
**Tool:** Claude or Comet | **Time:** ~15-30 min

1. List everything that needs fixing
2. Open `03_prompts/templates/PROMPT_refiner_ui.md`
3. Run one fix at a time
4. Save each version: output_v2.html, output_v3.html...
5. Log all refinement prompts in `03_prompts/projects/{name}/prompt_04_refinements.md`

Done when: Output looks right, works correctly, fits on screen.

---

## STEP 5 — Write SOP (Agent 5)
**Tool:** Claude or Comet | **Time:** ~10 min per piece

1. Open `03_prompts/templates/PROMPT_sop_writer.md`
2. Choose: GitHub README / Medium / LinkedIn / Gumroad guide
3. Paste MY_CONTEXT.md + BRIEF.md + prompt summaries
4. Run and save to `04_sop_outputs/{name}/`

Done when: At least one publishable piece of content is ready.

---

## STEP 6 — Log and Close
1. Add entry to `01_memory/PROJECT_LOG.md`
2. Add new lessons to `01_memory/LESSONS_LEARNED.md`
3. Commit everything to GitHub

---

## SHORTCUTS
- Already have context? Skip Step 1, start at Step 2
- Already have master prompt? Skip Steps 1-2, start at Step 3
- Project done, need SOP only? Run Step 5 only

---

## PIPELINE DIAGRAM

```
[YOUR IDEA]
     |
[AGENT 1 - Perplexity]  -->  prompt_01_context.md
     |
[AGENT 2 - ChatGPT]     -->  prompt_02_json_master.md
     |
[AGENT 3 - Claude]      -->  output_v1.html
     |
[AGENT 4 - Claude/Comet] --> output_vFINAL.html
     |
[AGENT 5 - Claude/Comet] --> 04_sop_outputs/{project}/
     |
[LOG] PROJECT_LOG.md + LESSONS_LEARNED.md + GitHub commit
```
