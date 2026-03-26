# SKILL: JSON Structuring for AI Workflows

## What Is This Skill?
JSON structuring is the practice of organizing your AI project ideas, file systems, and agent plans into clean JSON format — making them machine-readable and easy to reuse.

---

## Why JSON?
- It is the language AI tools understand best
- It can be converted directly into folder structures, config files, or templates
- It helps you think in systems, not just notes

---

## Basic JSON Structure Pattern

```json
{
  "project_name": "my-ai-workflow-system",
  "version": "1.0",
  "folders": [
    {
      "name": "01_memory",
      "purpose": "Store context, lessons, and background",
      "files": ["MY_CONTEXT.md", "LESSONS_LEARNED.md"]
    },
    {
      "name": "02_skills",
      "purpose": "Reusable skill guides",
      "files": ["SKILL_prompt_layering.md", "SKILL_json_structuring.md"]
    }
  ]
}
```

---

## How To Build JSON in Claude

### Step 1: Describe your structure in plain English
> "I have a folder system with memory files, skill guides, prompts, and SOP outputs. Each folder has 2-3 files."

### Step 2: Ask Claude to convert it
> "Turn this description into a clean JSON structure I can use as a project template."

### Step 3: Validate and refine
> "Now add a 'description' field to each file entry explaining what it contains."

---

## Common Mistakes To Avoid
- Trailing commas in JSON (will break the structure)
- Nesting too deeply (keep it 3 levels max for readability)
- Not labeling the purpose of each section
- Forgetting to save the JSON before moving to the next layer

---

## Steve's JSON Workflow
1. Describe the project in 3-5 sentences
2. Paste into Claude: "Convert this into a folder/file JSON structure"
3. Review and add any missing folders
4. Save the JSON to `00_meta/AGENT_PLAN.md` or as its own file
5. Use the JSON as reference when creating each file

---

## Related Files
- `00_meta/AGENT_PLAN.md` — the master plan (JSON-inspired structure)
- `02_skills/SKILL_prompt_layering.md` — how to layer prompts
- `03_prompts/PROMPT_claude_json_builder.md` — ready-to-use JSON prompt
