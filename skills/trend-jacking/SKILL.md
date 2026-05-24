---
name: trend-jacking
description: When the user wants to create content around a trending topic, news event, or cultural moment. Also use when the user says "trend-jack this," "write something about this news," "make content about what's happening," "reactive content," "hot take on X," "I want to comment on this trend," "turn this trending thing into content," or shares a link to a trending topic.
---

# Trend-Jacking

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `cta-style.json`

You help users create timely content that connects a trending topic to their brand's POV — fast, on-brand, and without looking desperate or off-topic.

## Context Check

Read `.agents/brand-voice.md` immediately. Trend-jacking lives and dies on brand fit. The biggest mistake is attaching the brand to a trend that has nothing to do with the brand's world.

## The Trend-Jacking Test

Before writing anything, run the trend through this filter:

**Relevance:** Does this trend genuinely connect to the brand's space, audience, or content pillars? (Not: "can we make it connect?" but "does it already connect?")

**Speed:** Is it still early enough to be timely? Most trends have a 24–72 hour window. After that, it reads as late.

**Tone fit:** Is the trend lighthearted, serious, controversial, technical? Does that match the brand's voice?

**Risk:** Is there political, cultural, or ethical risk in attaching the brand's name to this? When in doubt, don't.

If the trend fails any of these: tell the user directly. "This trend doesn't fit well for these reasons. Here's an alternative angle or a different trend to consider."

## Trend-Jacking Approaches

### The POV Play
"Here's my take on [trend] that connects to [brand topic]."
Best for: News, cultural moments, industry shifts.
Structure: What's happening → why it matters in the brand's context → the specific insight or implication

### The Analogy Bridge
Use the trending topic as a metaphor for something in the brand's space.
"[Trending thing] is basically [brand topic], and here's what that teaches us."
Risk: Can feel forced. Only use when the analogy is genuinely tight.

### The Contrarian Response
"Everyone is saying X about [trend]. I think Y."
Best for: Industry news, thought leader takes, predictable takes from big voices.
Risk: Contrarian for sport is transparent. Only if the POV is genuine.

### The Practical Application
"[Trend] is happening. Here's what that means for [audience] in practical terms."
Best for: Industry news, platform changes, market shifts.
Structure: The trend → specific implications for the audience → what to do about it

### The Humor / Culture Play
Use a trending meme, format, or cultural reference to deliver an on-brand message.
Best for: Brands with lighter voices. Avoid if brand is more serious/professional.
Risk: Memes age fast. Don't explain the joke.

## Speed Workflow

Trend-jacking is time-sensitive. Compress the process:

1. Confirm the trend is relevant and timely (2 min)
2. Pick the approach type (1 min)
3. Draft — one pass, fast (10–15 min)
4. Edit for banned words and voice (5 min)
5. Publish

Skip the brief. Skip multiple rounds. The cost of being late outweighs the cost of imperfection.

## Output

Deliver:
1. **Relevance verdict** (yes / conditional / no + reason)
2. **Recommended approach** with rationale
3. **Draft** — formatted for the platform (LinkedIn / X / Instagram / newsletter)
4. **Note on timing** — "Post within [X hours] for maximum relevance"

```
TREND: [Topic]
Relevance: [Yes / Conditional / No]
Reason: 
Approach: 
Platform: 
Timing: 

---

DRAFT:
[Content, formatted for platform]

---

ALTERNATIVE ANGLE (if main approach feels weak):
```

## What to Avoid

- **Tragedy jacking:** Never attach a brand to a tragedy, disaster, or death — even to express sympathy, unless it's genuinely relevant (e.g., an industry figure passes)
- **Political partisanship:** Unless the brand explicitly has a political stance, stay out
- **Late-to-trend posting:** A trend-jack posted 3 days late is worse than not posting
- **Forcing the connection:** "This reminds us that... [unrelated brand message]" is transparent and cringeworthy

## Related Skills

- `linkedin-post-writer` — most trend-jacking ends up as a LinkedIn post
- `x-writer` — X is the fastest platform for reactive content
- `content-editor` — quick voice QA before posting
- `editorial-calendar` — build reactive slots into the regular calendar
