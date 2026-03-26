# PROJECT: Amazon Fulfillment Center BPMN Dashboard

## Project Overview
**Project Name:** Amazon Fulfillment Center Interactive BPMN Workflow Dashboard
**Status:** Completed (v1.0)
**Built Using:** Claude AI (artifact), HTML, CSS, JavaScript
**Stored At:** Claude AI conversation + GitHub repo

---

## What This Project Is
An interactive web-based dashboard that visualizes the complete workflow of an Amazon Fulfillment Center using BPMN (Business Process Model and Notation) concepts.

The dashboard shows:
- All major departments and processes in one screen
- Interactive nodes that can be clicked and moved
- Color-coded process categories
- Auto-fit zoom so the full diagram is visible without manual zooming

---

## How This Project Was Built (The Process)

### Phase 1 — Ideation (ChatGPT)
- Used ChatGPT to explore what an Amazon Fulfillment Center workflow looks like
- Identified the major departments: Receiving, Stowing, Picking, Packing, Shipping, Returns
- Explored what BPMN elements would represent each stage

### Phase 2 — JSON Structuring (Claude)
- Took the ChatGPT ideas into Claude
- Asked Claude to build a JSON-like structure of all workflow nodes and connections
- Defined node types, labels, positions, and connections

### Phase 3 — Building the Dashboard (Claude Artifact)
- Asked Claude to build a full interactive HTML dashboard
- Iterated through multiple refinements:
  1. First build: basic diagram
  2. Refinement 1: Auto-fit zoom so everything is visible at a glance
  3. Refinement 2: Reduced node sizes for better proportions
  4. Refinement 3: Nodes unlocked for drag-and-drop interaction

### Phase 4 — Saving to GitHub
- Uploaded all project files to `github.com/Steve0a/my-ai-workflow-system`
- This project file saved under `06_projects/`

---

## Key Features of the Dashboard

| Feature | Description |
|---------|-------------|
| Auto-fit zoom | Entire workflow visible without zooming in/out |
| Interactive nodes | Click nodes for details, drag to reposition |
| Color coding | Each process type has its own color |
| Process connections | Arrows show flow between departments |
| Responsive layout | Works on different screen sizes |

---

## Lessons Learned From This Project
1. Starting with ChatGPT for ideas and Claude for building is an effective 2-tool workflow
2. Iterating in small steps (ask, review, refine) gives better results than asking for everything at once
3. Auto-fit zoom is essential for complex diagrams — always include it
4. Saving the build process as a project file helps you recreate it later

---

## How To Reuse This For Another Project
1. Copy this file and rename it (e.g., `PROJECT_hospital_workflow.md`)
2. Update the project overview section
3. Follow the same 4-phase process (Ideation → Structure → Build → Save)
4. Replace the Amazon-specific content with your new domain

---

## Related Files
- `00_meta/AGENT_PLAN.md` — overall system plan
- `05_chain_commands/CHAIN_full_pipeline.md` — chain commands that run this workflow
- `07_templates_master/MASTER_workflow_template.md` — reusable template for new projects
