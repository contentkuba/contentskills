---
name: content-brief
description: When the user wants to plan a piece of content before writing it. Also use when the user says "brief for this post," "plan this article," "content plan for X," "what angle should I take," "outline this," "I want to write about X, help me plan it," or provides a topic and wants structure before drafting. Run before blog-post-writer or seo-content-writer for best results.
---

# Content Brief

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `audience.json`
- `content-pillars.json`

**Also load:**
- `seo-keywords.json`

You help users create a focused, actionable content brief before writing — so the writing is faster, more strategic, and less likely to miss the mark.

## Context Check

Read `.agents/brand-voice.md` and `.agents/audience-persona.md` before asking questions. Use existing context and only ask for what's missing.

## When to Use a Brief

A brief is necessary when:
- The content is 500+ words
- The content has a strategic purpose (SEO, lead gen, authority)
- Multiple people are involved (writer + editor, or AI + human)
- The topic could go in many directions and you need to pick one

For quick posts and captions, skip the brief and go straight to the platform skill.

## Brief Interview

Ask in conversation, not all at once.

### The Piece
- Topic or working title
- Format: blog post / newsletter / LinkedIn article / YouTube script / other
- Approximate length goal
- Deadline or urgency

### The Goal
- What's the primary goal? (SEO traffic / email signups / social shares / sales / authority building)
- What's the one thing you want the reader to *do* after reading?
- What's the one thing you want the reader to *believe* after reading?

### The Angle
- What's the specific angle or POV? (not just "content marketing" but "why content marketing fails for B2B SaaS founders")
- What's the counterintuitive or surprising element?
- What would make someone who knows this topic well still want to read it?

### The Reader
- Who specifically is this for? (use audience persona if set)
- What do they already know about this topic?
- What do they get wrong about it?
- What do they *wish* someone would say about it?

### Research & Sources
- Are there specific data points, studies, or quotes to include?
- Are there competing pieces on this topic? What angle will differentiate this one?
- Are there personal stories or case studies to draw from?

### SEO (if applicable)
- Primary keyword
- Secondary keywords / related terms
- Search intent: informational / navigational / commercial / transactional

## Output: Content Brief

```markdown
# Content Brief: [Working Title]

## Overview
- Format: 
- Goal: 
- Target length: 
- Due: 

## The Reader
- Who: 
- Awareness level: 
- What they get wrong: 
- What they want to hear: 

## The Angle
- Core argument/POV: 
- Counterintuitive element: 
- Differentiation from existing content: 

## Outline
### Hook / Opening
[approach — story, stat, bold claim, question]

### Section 1: [H2]
- Key point: 
- Evidence/example: 

### Section 2: [H2]
- Key point: 
- Evidence/example: 

### Section 3: [H2]
- Key point: 
- Evidence/example: 

### Conclusion / CTA
- What to leave them with: 
- CTA: 

## SEO (if applicable)
- Primary keyword: 
- Secondary keywords: 
- Search intent: 
- Meta description direction: 

## Voice Notes
- Tone for this piece: 
- What to avoid: 
- Reference examples: 

## Research Needed
- [ ] 
- [ ] 
```

## Related Skills

- `content-research` — runs before or alongside the brief to find angles and data
- `blog-post-writer` — use the brief as input for the full draft
- `seo-content-writer` — SEO-specific writing, brief feeds directly in
- `audience-persona` — informs the reader section of every brief
