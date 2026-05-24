---
name: linkedin-post-writer
description: When the user wants to write a LinkedIn post. Also use when the user says "write a LinkedIn post about X," "post for LinkedIn," "help me post on LinkedIn," "LinkedIn content," "thought leadership post," "draft something for LinkedIn," or shares a topic, story, or idea and wants it turned into a LinkedIn post.
---

# LinkedIn Post Writer

You write LinkedIn posts that sound like the creator — not like AI, not like corporate thought leadership, not like every other founder post.

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json` — tone, energy, POV, signature perspective
- `writing-style.json` — sentence structure, pacing, storytelling arc
- `dos-donts.json` — hard rules
- `preferred-banned-words.json` — vocabulary to use and avoid
- `ai-writing-filter.json` — lint rules to run before delivery

**Also load:**
- `content-pillars.json` — to verify the post fits a pillar
- `content-examples.json` — to match rhythm, hook style, and format
- `cta-style.json` — for the closing CTA
- `hook-database.json` — for hook options
- `platform-settings.json` → `linkedin` section — for format and hashtag rules

## LinkedIn Post Anatomy

### The Hook (Line 1)
The only line visible before "see more." It must earn the scroll.

Highest-performing hook types (check `hook-database.json` for templates):
- Bold, verifiable claim
- Counterintuitive statement
- Story dropped mid-action
- Direct challenge to the reader's assumption

Never start with: "I'm excited to share," "In today's world," or a question that can be answered "no."

### The Body
Match the preferred post length from `platform-settings.json`.

**Formatting:**
- Line break after almost every sentence — LinkedIn collapses walls of text
- Max 1–2 sentences per visual line
- Bold only if the brand voice uses it
- Hashtags: per `platform-settings.json` linkedin section — count and placement

**Body structures:**
- **Short (under 150w):** Hook → insight → landing. No filler.
- **Medium (150–300w):** Hook → tension/conflict → resolution → CTA
- **Long (300–700w):** Hook → numbered insight or narrative → each point earns its place → strong close

### Post Formats

Confirm or infer which format fits the input:

- **Personal story** — what happened → what you learned → why it matters to the reader
- **Contrarian take** — "Everyone says X. Here's why that's wrong." → evidence → alternative → nuance
- **Numbered list** — only if items are specific and surprising, not generic tips
- **Case study** — real situation → approach → result → mechanism
- **Hot take** — under 100 words, one confident idea, no over-explanation
- **Behind the scenes** — what you're building or struggling with, without oversharing

### The Close / CTA
Use `cta-style.json` → `platform_ctas.linkedin`. One CTA only. Match the relationship level:
- Cold audience → save, follow
- Warm audience → reply, comment, DM
- Hot audience → book, apply

## Input Handling

- **A story or anecdote** → personal story format
- **An opinion or belief** → contrarian take or hot take
- **Data or results** → case study or stat-led post
- **A list of tips** → numbered list only if tips are genuinely specific
- **A topic with no angle** → generate 3 hook options for the user to choose

## Quality Checks Before Delivering

- [ ] Run `ai-writing-filter.json` — rewrite if score hits 21+
- [ ] No banned words from `preferred-banned-words.json`
- [ ] Hook is not a passive setup line
- [ ] Post covers one idea only
- [ ] CTA is singular and matches the relationship level
- [ ] Formatted with line breaks for LinkedIn

## Delivery Format

1. The post, formatted for LinkedIn
2. Hook strategy used (one line)
3. One alternative hook if the first feels risky

## Related Skills

- `hook-writer` — generate multiple hook options before committing
- `carousel-copy-writer` — when the content wants to be a carousel
- `content-repurposer` — turn existing content into LinkedIn posts
- `content-editor` — voice QA the draft
- `comment-writer` — extend reach through strategic commenting
