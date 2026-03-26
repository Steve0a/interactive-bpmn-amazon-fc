# PROMPT: Claude JSON Builder

## Purpose
Use this prompt in Claude to convert your brainstorm, ideas, or rough notes into a clean JSON-based project structure.

---

## When To Use This Prompt
- After doing your ChatGPT ideation session
- When you want to plan a new project folder system
- When you want to convert a messy idea into something organized

---

## The Prompt Template

Copy and paste this into Claude:

```
I want to build an organized system for [DESCRIBE YOUR PROJECT IN 1-2 SENTENCES].

Here are my rough ideas and notes:
[PASTE YOUR CHATGPT OUTPUT OR NOTES HERE]

Please do the following:
1. Create a clean JSON structure with folders and files
2. Each folder should have a "name", "purpose", and "files" array
3. Each file in the array should have a "filename" and "description"
4. Keep it practical — only include what I actually need
5. Format it as valid JSON I can copy directly

After the JSON, give me a plain English summary of the structure in 3-5 bullet points.
```

---

## Example Filled Prompt

```
I want to build an organized system for my personal AI workflow — a reusable system I can use for future projects on Gumroad and Medium.

Here are my rough ideas and notes:
- I want memory files to store my context
- Skills files that teach me techniques
- Prompt templates I can reuse
- SOP outputs written in simple language
- Chain commands to run multi-step tasks
- A master template I can clone for new projects

Please do the following:
1. Create a clean JSON structure with folders and files
2. Each folder should have a "name", "purpose", and "files" array
3. Each file in the array should have a "filename" and "description"
4. Keep it practical — only include what I actually need
5. Format it as valid JSON I can copy directly

After the JSON, give me a plain English summary of the structure in 3-5 bullet points.
```

---

## Tips For Better Results
- Be specific about what each section is FOR, not just what it is
- Mention if you want it to be reusable or project-specific
- Tell Claude the audience (just for you, or to sell/share later?)
- After you get the JSON, ask: "Now add a README.md to each folder with a short description"

---

## Related Files
- `02_skills/SKILL_json_structuring.md` — the theory behind this prompt
- `03_prompts/PROMPT_chatgpt_ideation.md` — use this BEFORE this prompt
- `00_meta/AGENT_PLAN.md` — where to save the output
