---
name: case-study-writer
description: When the user wants to write a case study. Also use when the user says "write a case study," "client story," "success story," "customer story," "results story," "before and after story," "document this project," or wants to turn a real client or project outcome into content.
---

# Case Study Writer

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `brand-identity.json`

You write case studies that are worth reading — built on specificity, not vague claims, and structured to both prove results and tell a story.

## Context Check

Read `.agents/brand-voice.md`. Case studies carry the brand's credibility. Voice consistency matters.

## Why Case Studies Fail

Most case studies are useless because they're:
- Too vague ("We helped a client improve their results significantly")
- Too feature-focused (what the tool does, not what changed for the client)
- Too corporate (written for a boardroom, not a potential buyer)
- Missing the story (numbers without context are just numbers)

A great case study is a story with receipts.

## Case Study Formats

**Full Case Study**
1,000–2,000 words. Covers the full arc: situation, problem, process, results, lessons. Best for website, sales enablement, long-form blog.

**Mini Case Study / Story Post**
300–600 words. The core insight and results, lightly narrated. Best for LinkedIn, newsletter, sales decks.

**Snapshot**
50–150 words. The situation + 2–3 specific results. Best for testimonial pages, proposals, slide decks.

**Social Proof Pull Quote**
One sentence, attributed. Extracted from the full case study.

Ask or infer which format is needed.

## Case Study Interview

Collect the real story — don't write from vague summaries.

### The Client / Subject
- Who was the client or subject? (Can be anonymous if needed: "a B2B SaaS founder" / "a 3-person agency")
- What's their context? (industry, size, stage, relevant background)

### The Before
- What was the situation before working together or before implementing the change?
- What was the specific problem or pain point?
- What had they already tried? What hadn't worked?
- What was at stake?

### The Process
- What was done? (the actual approach, not just the category)
- What was the key decision or insight that made the difference?
- Were there any surprises, pivots, or moments of difficulty?

### The After
- What were the specific, measurable results?
- In what timeframe?
- What changed qualitatively (beyond numbers)?
- What would the client say now that they wouldn't have said before?

### The Lesson
- What can a reader do differently or think about differently because of this story?
- What would you do again? What would you change?

## Case Study Structure

### Headline
Not: "How [Brand] Helped [Client]"
Yes: "[Specific result] in [timeframe]: How [Client type] [achieved specific outcome]"

Example: "From 0 to 4,200 newsletter subscribers in 90 days: How a solo founder built an audience before launching"

### The Hook
The most compelling result or the most relatable problem. Don't save the good stuff for the end.

### The Situation
Set the scene. Who is this person/company? What were they trying to do? Keep it brief — just enough to make the reader identify.

### The Problem
Get specific about what wasn't working and why. This is where readers recognize themselves.

### The Approach
What was done and why. Not a product pitch — a process explanation. The insight or decision that changed things.

### The Results
Numbers first, then context. Specific and time-bounded:
- Not: "significantly increased revenue"
- Yes: "MRR grew from $3,200 to $11,400 in 4 months"

List 2–4 key results. Then the qualitative shift (what it meant for the client beyond the numbers).

### The Quote
One strong client quote that captures the emotional truth of the transformation.

### The Lesson
What can the reader apply? This is what makes the case study content, not just a sales document.

## Output Format

```
CASE STUDY: [Headline]
Format: [Full / Mini / Snapshot]

---

HEADLINE: 
SUBHEADLINE: [Optional]

HOOK:
[The most compelling result or most relatable problem — 2–3 sentences]

THE SITUATION:
[Who + context — 1 short paragraph]

THE PROBLEM:
[What wasn't working, what they'd tried — 1–2 paragraphs]

THE APPROACH:
[What was done and why — 1–2 paragraphs, process-focused]

THE RESULTS:
- [Specific result 1]
- [Specific result 2]
- [Specific result 3]

[Qualitative shift — 1–2 sentences]

CLIENT QUOTE:
"[Specific, real-sounding quote]"

THE LESSON:
[What the reader can apply — 1 short paragraph]

CTA: [What to do if this resonates]
```

## Related Skills

- `testimonial-extractor` — pull the quote from the case study
- `content-repurposer` — adapt the case study into LinkedIn post, carousel, newsletter
- `launch-content-planner` — case studies as proof during launch week
