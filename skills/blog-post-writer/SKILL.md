---
name: blog-post-writer
description: When the user wants to write a blog post or long-form article. Also use when the user says "write a blog post," "write an article," "long-form content," "write a piece on X," "blog content," "thought leadership article," or has a topic and wants a full draft.
---

# Blog Post Writer

## Context Check

Before doing anything, load brand context in this order:
1. `.agents/brand-voice.md`
2. `.claude/brand-voice.md` (fallback)

If neither exists, run the `brand-voice` skill first, then return to this workflow.

## Reference Files

Read these before writing. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `audience.json`
- `content-pillars.json`
- `cta-style.json`
- `platform-settings.json` (blog section)
- `seo-keywords.json`

---

## Workflow

Wait for the user to provide a keyword or title before beginning. Then follow these three steps in order.

---

### Step 1: Competitive Analysis

Search the keyword or title using web search. Analyze the first 5 results that appear. For each result, identify what it does well and what it is missing or could improve. Look for gaps in depth, missing subtopics, weak structure, lack of examples, outdated information, or anything a stronger piece of content could do better.

Present the analysis using this exact structure for each source:

```
1. [Name of the source]

1.1. Useful insights:

- [insight 1]
- [insight 2]
- [insight 3]

1.2. What is missing:

- [missing insight 1]
- [missing insight 2]
- [missing insight 3]
```

Repeat for all 5 sources.

After the competitive analysis, ask: "Is this analysis thorough enough?"

- If the user replies "Yes" - proceed to Step 2.
- If the user replies "No" - ask what is missing, incorporate their feedback, then proceed.

---

### Step 2: Article Outline

Once the competitive analysis is approved, write a full article outline. Use the insights gathered from the competitive analysis. Fill in any gaps or missing information that the competition failed to cover.

Do not start the outline with an introduction section. Begin directly with the first H2 subheading.

Use this exact structure for each section:

```
H2 - [Subheading Title Suggestion]

Section word count: [~X words]

Section detail: [Brief description of what this section covers and its purpose in the article]

Topics to touch on:

- [topic 1]
- [topic 2]
- [topic 3]
```

Repeat this structure for every H2 section in the outline.

---

### Step 3: Writing the Article

After the outline is approved, write the full article section by section. The user will prompt each section with: "Write this section: H2..."

Apply all reference files (voice, writing style, dos/don'ts, banned words) while following these writing rules:

**Headlines and structure**
- Craft a precise, benefit-driven headline. Promise a clear outcome, avoid vagueness, make the value immediately understandable.
- Do not start the outline or article with an introduction section. Begin directly with the first H2.
- Include the primary keyword in H2 headers where natural.

**Opening**
- Deliver value early. State the core insight, answer, or framework within the first section so readers gain immediate clarity even if they skim.

**Readability**
- Structure for scannability: short paragraphs, descriptive subheadings, bullet points, numbered lists, and clear section breaks.
- Keep paragraphs concise. Aim for tight, focused sections that communicate one idea at a time.
- Prioritize clarity over cleverness. Write in simple, direct language. Avoid filler, jargon, and unnecessary complexity.

**Depth and credibility**
- Add original insight. Include real examples, case observations, frameworks, data, or lived experience to differentiate the content from generic summaries.
- Demonstrate expertise and credibility. Reference reputable sources when needed, explain reasoning clearly, and show depth of understanding rather than repeating surface-level information. Use web search if needed.

**SEO and AI optimization**
- Optimize for both humans and AI systems. Use natural keyword placement, clear semantic structure, concise definitions, and answer-focused sections that are easy to extract and summarize.
- Follow core SEO fundamentals. Include the primary keyword in H2 headers. Use the keywords from `seo-keywords.json` where natural.

---

## Formatting Rules

Apply to all responses - competitive analysis, outline, and written sections:

- Do not use en-dashes or em-dashes anywhere in your response.
- Use only standard ASCII punctuation (hyphens, commas, periods, colons, semicolons, parentheses, etc.).
- Do not use smart quotes or curly quotes. Use only straight quotes (" and ').

---

## Related Skills

- `content-brief` - create a brief before starting the competitive analysis
- `seo-content-writer` - SEO-specific optimization layer on top of blog writing
- `content-editor` - review and edit a completed draft
- `content-repurposer` - repurpose the finished article into other formats
- `hook-writer` - craft a stronger opening hook for the article
