# My AI Workflow System

**Owner:** Steve0a | **Created:** March 2026 | **Status:** Active

> A personal, reusable 5-agent pipeline for building AI-powered projects — from idea to published output.

---

## What This Is

Every time I start a new project (dashboard, BPMN diagram, website, presentation, PDF guide), I follow the same folder structure and the same chain of prompts. Only the subject changes.

Think of it like a recipe book. The recipe stays the same. You just swap the ingredients.

---

## The 5-Agent Pipeline

| # | Agent | Job | Tool |
|---|-------|-----|------|
| 1 | **Context Collector** | Research and gather business info | Perplexity |
| 2 | **Prompt Architect** | Build structured JSON master prompt | ChatGPT |
| 3 | **Builder** | Build the actual output (HTML, dashboard, etc.) | Claude |
| 4 | **Refiner** | Fix and polish until it looks right | Claude / Comet |
| 5 | **SOP Writer** | Write the guide, README, article, Gumroad PDF | Claude / Comet |

---

## Folder Structure

```
my-ai-workflow-system/
├── 00_meta/           # What this system is
├── 01_memory/         # Who I am, preferences, project history
├── 02_skills/         # How-to guides for specific techniques
├── 03_prompts/        # All reusable and project-specific prompts
├── 04_sop_outputs/    # Final published content
├── 05_chain_commands/ # Step-by-step pipeline instructions
├── 06_projects/       # One folder per project
└── 07_templates_master/ # Master templates for new projects
```

---

## Case Study #1 — Amazon Fulfillment Center BPMN

**What I built:** An interactive HTML dashboard showing the full Amazon FC end-to-end workflow with BPMN-style design, RACI cards, swimlanes, color-coded roles, zoom/pan, and clickable side panels.

**Tools used:** Perplexity (context) → ChatGPT (JSON prompt) → Claude (build + refine)

**Folder:** `06_projects/amazon_bpmn/`

---

## Golden Rule

> No agent starts from scratch. Every agent receives a file as input. Every agent saves a file as output. Nothing lives only in your head.

---

## How to Start a New Project

1. Copy `07_templates_master/NEW_PROJECT_KICKOFF.md`
2. Fill it in (5 minutes)
3. Follow `05_chain_commands/CHAIN_full_pipeline.md`
4. Done — your output + SOP are both saved

---

*Built by Steve0a | Park University Data Analytics*
