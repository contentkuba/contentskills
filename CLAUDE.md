# Content Skills — Agent Instructions

## What This Repo Is

This is a collection of content marketing skills for AI agents. Each skill is a markdown file that gives agents specialized knowledge and workflows for specific content tasks.

## How Skills Are Loaded

Skills are loaded when the user's request matches the skill's `description` trigger. The description field in each skill's YAML frontmatter is the primary matching mechanism — it must be specific and include the natural language phrases a user would use.

## The Brand Voice Rule

**Every skill in this repo reads `.agents/brand-voice.md` before doing anything.**

Check in this order:
1. `.agents/brand-voice.md`
2. `.claude/brand-voice.md` (fallback)

If neither exists, run the `brand-voice` skill first and create the file before proceeding with the original task. Do not generate content without brand voice context.

## Skill File Location

Skills live at:
```
skills/[skill-name]/SKILL.md
```

## Brand Context Files

User-specific context files live at:
```
.agents/brand-voice.md         # Brand voice, tone, banned words, examples
.agents/audience-persona.md    # Audience definition and psychology
.agents/content-strategy.md    # Content strategy (created by content-strategist skill)
```

## Version Checking

Once per session, on first skill use, check for updates:
- Fetch `VERSIONS.md` from the repo
- Compare against local skill files
- If 2+ skills have updates or any major version bump, notify the user at the end of the response

Non-blocking: `--- Content skills update available. Say "update skills" to update.`

## Skill Authoring Rules

When contributing or creating new skills:
- YAML frontmatter: `name` (matches directory) and `description` (1–1024 chars)
- H2 (##) for main sections, H3 (###) for subsections
- Under 500 lines per SKILL.md
- Always include: Context Check section, Related Skills section
- Description must include trigger phrases in natural language
- Every skill must reference the brand-voice check at the top

## Related

See `CONTRIBUTING.md` for PR guidelines.
See `README.md` for the full skill directory and installation instructions.
