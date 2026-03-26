# MASTER TEMPLATE: New AI Workflow Project

> Copy this entire folder structure to start a new project. Replace everything in [BRACKETS] with your own content.

---

## HOW TO USE THIS TEMPLATE

1. Create a new GitHub repo (e.g., `my-[project-name]-system`)
2. Copy this folder structure
3. Fill in each file using the prompts in `03_prompts/`
4. Save your context in `01_memory/` as you go
5. Document your completed project in `06_projects/`

---

## FOLDER STRUCTURE TO COPY

```
[PROJECT-NAME]/
├── README.md                          ← Project overview (fill in first)
├── 00_meta/
│   └── AGENT_PLAN.md                 ← Master plan and agent structure
├── 01_memory/
│   ├── MY_CONTEXT.md                 ← Your background and project context
│   └── LESSONS_LEARNED.md            ← What you learn as you build
├── 02_skills/
│   ├── SKILL_prompt_layering.md      ← How to layer prompts across AI tools
│   └── SKILL_json_structuring.md     ← How to build JSON structures
├── 03_prompts/
│   ├── PROMPT_chatgpt_ideation.md    ← Use in ChatGPT for brainstorming
│   └── PROMPT_claude_json_builder.md ← Use in Claude for structuring
├── 04_sop_outputs/
│   └── SOP_[process-name].md         ← Your documented processes
├── 05_chain_commands/
│   └── CHAIN_[workflow-name].md      ← Multi-step command chains
├── 06_projects/
│   └── PROJECT_[name].md             ← Completed project documentation
└── 07_templates_master/
    └── MASTER_workflow_template.md    ← This file — clone for new projects
```

---

## QUICK START CHECKLIST

### Before You Build
- [ ] I have a clear 1-sentence description of the project
- [ ] I know who this is for (just me, or to share/sell?)
- [ ] I have ChatGPT open for ideation
- [ ] I have Claude open for building

### Phase 1 — Ideation (15-30 mins)
- [ ] Used `PROMPT_chatgpt_ideation.md` in ChatGPT
- [ ] Saved the output to `01_memory/MY_CONTEXT.md`
- [ ] Identified 3-5 core components of the project

### Phase 2 — Structuring (15-30 mins)
- [ ] Used `PROMPT_claude_json_builder.md` in Claude
- [ ] Got a clean folder/file structure back
- [ ] Saved the structure to `00_meta/AGENT_PLAN.md`

### Phase 3 — Building (varies)
- [ ] Built each file one by one
- [ ] Tested/reviewed each output before moving on
- [ ] Saved lessons learned in `01_memory/LESSONS_LEARNED.md`

### Phase 4 — Save and Organize
- [ ] Created GitHub repo
- [ ] Uploaded all files
- [ ] Filled in `06_projects/PROJECT_[name].md`
- [ ] Updated README.md with final summary

---

## README TEMPLATE (paste into your README.md)

```markdown
# [PROJECT NAME]

## What Is This?
[1-2 sentence description]

## Who Is This For?
[Who would use or benefit from this]

## How To Use It
1. [Step 1]
2. [Step 2]
3. [Step 3]

## Folder Structure
[paste your folder list here]

## Built With
- ChatGPT (ideation)
- Claude AI (building)
- GitHub (storage)

## Author
Steve — [date]
```

---

## NOTES FOR REUSE
- This template is designed to work for ANY type of AI project
- Skills files (02_skills/) are reusable across all projects — don't recreate them
- Always fill in `01_memory/MY_CONTEXT.md` FIRST before building anything
- The chain commands in `05_chain_commands/` let you run the whole pipeline in one go

---

## Related Files
- `00_meta/AGENT_PLAN.md` — the master system architecture
- `05_chain_commands/CHAIN_full_pipeline.md` — automated pipeline commands
