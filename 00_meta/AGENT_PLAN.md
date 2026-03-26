# Agent Plan — The 5-Agent Pipeline

## Overview

This system uses 5 agents running in sequence. Each agent takes the previous agent's output as its input. You run them manually (copy-paste prompts) for now. Later this can be automated with n8n.

---

## Agent 1 — Context Collector

**Goal:** Gather all raw information about the topic or business you are building for.
**Runs in:** Perplexity
**Input:** Your rough idea / topic / company name
**Output:** `03_prompts/projects/{name}/prompt_01_context.md`
**Prompt file:** `03_prompts/templates/PROMPT_context_collector.md`

---

## Agent 2 — Prompt Architect

**Goal:** Take the context and turn it into a structured JSON master prompt.
**Runs in:** ChatGPT
**Input:** `prompt_01_context.md`
**Output:** `03_prompts/projects/{name}/prompt_02_json_master.md`
**Prompt file:** `03_prompts/templates/PROMPT_architect_master.md`

---

## Agent 3 — Builder

**Goal:** Build the actual deliverable from the master prompt.
**Runs in:** Claude
**Input:** `prompt_02_json_master.md`
**Output:** `06_projects/{name}/ASSETS/output_v1.html`
**Prompt file:** `03_prompts/templates/PROMPT_builder_html.md`

---

## Agent 4 — Refiner

**Goal:** Fix, adjust, resize, and polish the output.
**Runs in:** Claude / Comet
**Input:** Built file + your feedback
**Output:** `output_v2.html`, `v3.html`... + `prompt_04_refinements.md`
**Prompt file:** `03_prompts/templates/PROMPT_refiner_ui.md`

---

## Agent 5 — SOP Writer

**Goal:** Document the whole project in plain English for publishing.
**Runs in:** Claude / Comet
**Input:** All prompt files + final output + `01_memory/MY_CONTEXT.md`
**Output:** All content in `04_sop_outputs/{project}/`
**Prompt file:** `03_prompts/templates/PROMPT_sop_writer.md`

---

## Pipeline Flow

```
[YOUR IDEA]
    |
[AGENT 1 - Perplexity]  -->  prompt_01_context.md
    |
[AGENT 2 - ChatGPT]     -->  prompt_02_json_master.md
    |
[AGENT 3 - Claude]      -->  ASSETS/output_v1.html
    |
[AGENT 4 - Claude/Comet] --> ASSETS/output_vFINAL.html
    |
[AGENT 5 - Claude/Comet] --> 04_sop_outputs/{project}/
    |
[UPDATE] PROJECT_LOG.md + LESSONS_LEARNED.md
```

---

## Future: n8n Automation

Each agent becomes an n8n node. Files pass automatically. Trigger = fill in kickoff form.
