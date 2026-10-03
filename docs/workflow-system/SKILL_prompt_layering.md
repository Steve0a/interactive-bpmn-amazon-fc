# SKILL: Prompt Layering

## What Is This Skill?
Prompt layering is the technique of building a complex AI output in stages — each prompt builds on the output of the previous one.

---

## When To Use It
- When one prompt is too complex to handle everything
- When you need to move ideas from one AI tool to another (e.g., ChatGPT → Claude)
- When you want to refine, not regenerate

---

## The Layering Pattern

### Layer 1 — Ideation (ChatGPT)
**Goal:** Get raw ideas, brainstorm, explore possibilities.
**Prompt style:** Open-ended, creative, "what if" style.
**Example:**
> "I want to build a workflow system for AI projects. What are the key components I should include? Think broadly."

### Layer 2 — Structuring (Claude)
**Goal:** Take the ideas and turn them into structured JSON, markdown, or a plan.
**Prompt style:** "Here is the output from my last session. Now organize this into..."
**Example:**
> "Here is my brainstorm from ChatGPT. Turn this into a JSON structure with folders, files, and descriptions."

### Layer 3 — Building (Claude or Code Tool)
**Goal:** Take the structure and build actual files, code, or templates.
**Prompt style:** "Now build file X from the structure we created."

### Layer 4 — Review & Refine
**Goal:** Check the output, fix gaps, improve language.
**Prompt style:** "Review this and make it clearer / more reusable / easier to understand."

---

## Steve's Personal Pattern
1. ChatGPT: Big picture idea exploration
2. Claude: JSON structure + file planning
3. Claude: File-by-file content generation
4. GitHub: Store and organize everything
5. Dashboard/HTML: Visual representation

---

## Reuse Tips
- Save your Layer 1 output as a memory file before moving to Layer 2
- Always paste previous output at the top of your next prompt
- Label each layer clearly in your notes (e.g., "Layer 1 done - saved to MY_CONTEXT.md")

---

## Related Files
- `01_memory/MY_CONTEXT.md` — stores your current project context
- `03_prompts/PROMPT_chatgpt_ideation.md` — example Layer 1 prompts
- `03_prompts/PROMPT_claude_json_builder.md` — example Layer 2 prompts
