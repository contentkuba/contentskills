---
name: infographic-designer
description: When the user wants to create an infographic. Also use when the user says "make an infographic," "design an infographic," "visualize this data," "infographic about X," "turn this into an infographic," "visual summary," or wants to take a topic or data set and make it shareable as a graphic.
---

# Infographic Designer

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `content-pillars.json`
- `audience.json`

**Also load:**
- `visual-language.json`
- `brand-identity.json`

You produce complete infographic concepts and copy — the type, headline, structure, all text, and a designer brief — ready to hand to Canva, a designer, or an AI image tool.

## Context Check

Read `.agents/brand-voice.md`. Note any visual style preferences, color direction, or design references in the brand voice file.

## What This Skill Produces

This is a **copy and concept skill**, not a design tool. Output is:
1. Infographic type recommendation + rationale
2. Headline and subheadline
3. All body copy, section by section
4. A designer brief with layout, visual, and hierarchy guidance

The output can go directly into Canva, a designer's hands, or an AI image generation prompt.

## Infographic Type Selection

Identify the right type for the content before writing anything:

**List / Tips**
Content: discrete items without inherent order
Best for: "X ways to..." "X mistakes..." "X tools..."
Layout: vertical stack or grid

**Process / Steps**
Content: sequential, one leads to the next
Best for: how-to, workflows, methods
Layout: horizontal flow or numbered vertical

**Comparison**
Content: two or more things side by side
Best for: before/after, X vs. Y, option comparison
Layout: two or three columns, aligned attributes

**Timeline**
Content: chronological sequence of events
Best for: history, milestones, project stages
Layout: horizontal or vertical timeline

**Data / Statistics**
Content: numbers, percentages, research findings
Best for: research summaries, survey results, market data
Layout: data visualization (charts, big numbers, callouts)

**Pyramid / Hierarchy**
Content: layers of priority or dependency
Best for: frameworks, priority stacks, Maslow-style concepts
Layout: triangle or inverted triangle

**Hub and Spoke**
Content: one central idea with connected sub-ideas
Best for: ecosystems, related concepts, multi-factor topics
Layout: central circle with radiating elements

**Checklist**
Content: items with yes/no or done/not-done status
Best for: audits, readiness checks, habit trackers
Layout: vertical list with checkbox style

## Brief Interview

Ask only what's needed:
- What's the topic?
- What's the primary goal? (educate / persuade / entertain / share)
- Where will it be published? (LinkedIn / Instagram / blog / presentation)
- Are there specific data points or content to include, or should I generate the content?
- Are there brand colors, fonts, or style references?

## Infographic Copy Output

```
INFOGRAPHIC CONCEPT: [Title]
Type: [from list above]
Platform: 
Dimensions: [e.g., 1080x1350 for Instagram portrait, 1200x627 for LinkedIn]

---

HEADLINE: [Bold, benefit-driven, 6–10 words]
SUBHEADLINE: [Optional — adds context or intrigue, 10–15 words]

---

SECTION 1: [Label]
Copy: [concise — infographics live and die by brevity]
Visual note: [icon suggestion, chart type, or image direction]

SECTION 2: [Label]
Copy: 
Visual note: 

[...repeat for all sections]

---

FOOTER
Source/credit line: 
CTA / URL: 
Brand: 

---

DESIGNER BRIEF
Layout description: [prose description of the visual layout]
Color direction: [primary, secondary, accent — from brand voice or suggested]
Font direction: [if not already defined]
Hierarchy notes: [what to make big, what to make small]
Mood/reference: [2–3 adjectives or a reference style]
```

## Copy Rules for Infographics

- **Headlines on sections:** 2–5 words. Labels, not sentences.
- **Body copy per section:** 10–25 words max. If it needs more, it's not an infographic.
- **Numbers:** If there are statistics, make the number the hero. Big, bold, center.
- **No filler:** Every word is visible and costs design space. Ruthless editing required.

## Related Skills

- `content-research` — find data points and examples before designing
- `carousel-copy-writer` — when the content is better as slides than a single graphic
- `content-repurposer` — identify which existing content becomes infographics
- `seo-content-writer` — infographic as a linkable asset in a larger post
