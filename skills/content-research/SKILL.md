---
name: content-research
description: When the user wants to research a topic before writing. Also use when the user says "research this for me," "find angles on X," "what's already been written about X," "find data on X," "help me find a hook," "what's trending on this topic," "competitor content on X," or "I need sources for this piece." Run before content-brief or any long-form writer skill.
---

# Content Research

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `audience.json`
- `content-pillars.json`

**Also load:**
- `brand-identity.json`

You help users research a topic thoroughly before writing — finding angles, data points, competitor gaps, and audience language that makes content original and credible.

## Context Check

Read `.agents/brand-voice.md` and `.agents/audience-persona.md`. Use brand context to filter research toward relevant angles and away from off-brand approaches.

## Research Modes

Ask the user which mode they need, or infer from context:

### 1. Angle Research
Finding the right POV before writing anything. Best for: new topics, competitive spaces, contrarian pieces.

### 2. Data & Evidence Research
Finding stats, studies, and quotes to support a piece already being written.

### 3. Competitor Content Audit
What's already ranking or performing on this topic? What's missing?

### 4. Audience Language Mining
What exact words and phrases does the audience use? Where are they venting, asking questions, celebrating?

### 5. Trend Research
What's emerging or shifting on this topic right now?

## Research Process

### Step 1: Topic Clarification
Before researching, confirm:
- The specific topic (not just "content marketing" — what angle?)
- The platform/format this is for
- The audience (use persona if set)
- The goal (SEO / thought leadership / conversion)

### Step 2: Angle Mining
Generate 8–12 potential angles on the topic. For each angle, assess:
- Originality (has this been done to death?)
- Audience relevance (does it match the persona's actual problem?)
- Brand fit (does it align with the voice and POV?)
- Differentiation (what's the unique take?)

Present top 3 angles with rationale. Let user choose or combine.

### Step 3: Evidence & Data Points
For the chosen angle, find or suggest:
- Relevant statistics (with source quality assessment)
- Research studies or reports
- Case studies or real-world examples
- Expert quotes or attributable claims
- Counter-evidence (to make the argument more honest and interesting)

### Step 4: Audience Language
Pull exact language the audience uses:
- How do they describe the problem?
- What questions do they ask?
- What frustrations do they voice?
- What solutions have they tried and rejected?

Sources: Reddit, LinkedIn comments, Twitter/X threads, product reviews, community forums, YouTube comments.

### Step 5: Competitive Gap Analysis
For the chosen topic and angle:
- What's already ranking or performing?
- What perspective is missing from existing content?
- What angle would make an experienced reader still want to read this?
- What format is underserved (e.g., everyone's writing listicles, no one's doing case studies)?

## Research Output

Deliver a research package structured as:

```markdown
# Research Package: [Topic]

## Chosen Angle
[The specific POV and why it was chosen]

## Key Data Points
- [Stat/finding] — [Source] — [Quality: primary/secondary/anecdotal]
- [Stat/finding] — [Source] — [Quality]
- [Stat/finding] — [Source] — [Quality]

## Strong Examples & Cases
- [Example] — [Why it's relevant]
- [Example] — [Why it's relevant]

## Audience Language
Words/phrases they use:
- "..."
- "..."

Questions they ask:
- "..."
- "..."

Frustrations:
- "..."

## Competitive Landscape
- What exists: [summary]
- What's missing: [the gap this piece fills]
- Differentiation angle: [how to be different]

## Rejected Angles (and why)
- [Angle] — [Why it's overdone/wrong fit/off-brand]

## Suggested Outline Direction
[Brief bullet structure based on research — feeds into content-brief]
```

## Research Quality Rules

- Flag the difference between primary research (studies, surveys), secondary sources (articles citing studies), and anecdotal/opinion
- Never fabricate statistics — if a specific number is needed and not found, say so
- Prioritize recent data (last 2 years) for fast-moving topics; older data is fine for evergreen topics
- Note when a stat is widely cited but original source is unclear

## Related Skills

- `content-brief` — research feeds directly into the brief
- `trend-jacking` — uses real-time research to find timely angles
- `seo-content-writer` — research informs keyword and intent strategy
- `blog-post-writer` — research package becomes the raw material for the draft
