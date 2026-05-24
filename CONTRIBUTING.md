# Contributing to Content Skills

Contributions welcome. Here's how to add or improve a skill.

## Adding a New Skill

1. Create a directory: `skills/[skill-name]/`
2. Create `SKILL.md` inside it
3. Follow the skill format below
4. Add the skill to `README.md` in the correct category
5. Add the skill to `VERSIONS.md`
6. Open a PR

## Skill Format

```markdown
---
name: skill-name
description: When the user wants to [task]. Also use when the user says "[phrase 1]," "[phrase 2]," or "[phrase 3]."
---

# Skill Title

One sentence on what this skill does.

## Context Check

Read `.agents/brand-voice.md` before [doing anything]. If it doesn't exist, run the `brand-voice` skill first.

## [Main Section]

...

## Related Skills

- `skill-name` — [why it's related]
- `skill-name` — [why it's related]
```

## Rules

- `name` must match the directory name exactly
- `name`: lowercase, alphanumeric, hyphens only, 1–64 characters
- `description`: 1–1,024 characters — include the natural language phrases a user would actually say
- Every skill must have a **Context Check** section that reads brand-voice first
- Every skill must have a **Related Skills** section
- Keep SKILL.md under 500 lines — move detailed reference material to a `references/` subfolder
- Use H2 (`##`) for main sections, H3 (`###`) for subsections

## Improving an Existing Skill

- Open an issue describing the improvement
- Or submit a PR directly with a clear description of what changed and why
- For significant rewrites, open an issue first to discuss

## What Makes a Good Skill

A good skill:
- Solves a specific, recurring content task
- Has a description that clearly distinguishes it from similar skills
- Reads brand-voice and applies it throughout
- Gives the agent a process, not just knowledge
- Has clear output formats the user can use immediately
- Doesn't duplicate what another skill already covers

## What We Don't Accept

- Skills that ignore the brand-voice requirement
- Skills that are just lists of tips (no process)
- Skills duplicating existing skills without clear differentiation
- Skills without the required frontmatter format
