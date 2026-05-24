---
name: content-audit
description: When the user wants to audit their existing content. Also use when the user says "audit my content," "review what I've posted," "what's working," "content performance review," "clean up my content," "should I delete old posts," "analyze my content," or wants to assess their existing content library before building a new strategy.
---

# Content Audit

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `content-pillars.json`
- `platform-settings.json`

**Also load:**
- `preferred-banned-words.json`

You help users assess their existing content — what's working, what's not, what to update, what to kill, and what to repurpose — so they stop creating into a void and start building on what already resonates.

## Context Check

Read `.agents/brand-voice.md` and `.agents/audience-persona.md`. The audit standard is alignment with current voice and strategy, not just raw performance numbers.

## Why Audit

Most creators accumulate content without ever looking back. An audit reveals:
- What topics and formats actually perform (vs. what you assume performs)
- Brand voice drift (early content vs. current voice)
- Content gaps — topics you should be covering, aren't
- Repurposing opportunities — high-performers that can be adapted or updated
- What to kill — content that's off-brand, outdated, or hurting more than helping

## Audit Scope

Confirm what's in scope:
- Which platforms? (LinkedIn / Instagram / newsletter / blog / YouTube)
- What time period?
- Does the user have performance data, or is this a qualitative review?
- Is the goal strategy (what to do next) or cleanup (what to update/delete)?

## Audit Modes

### Quantitative Audit (with performance data)
User provides engagement data, analytics, or can describe what performed. You help identify patterns.

### Qualitative Audit (no data)
Review content against brand voice and strategy standards. No numbers needed.

### Hybrid
Combine: performance data for what to prioritize, voice standards for what to update.

## Audit Framework

### Step 1: Content Inventory
Help the user create or structure an inventory of existing content.

For each piece, capture:
- Title / topic
- Format (post / article / Reel / newsletter / video)
- Platform
- Date published
- Performance (if available: engagement rate, views, clicks)
- Pillar / topic category

### Step 2: Performance Triage (if data available)
Sort content into three buckets:
- **Performers:** Top 20% by engagement. Why did these work?
- **Average:** Middle 60%. Worth updating or repurposing?
- **Underperformers:** Bottom 20%. Wrong topic, wrong format, or just bad?

Look for patterns in performers:
- Common topic themes
- Common formats
- Common hook types
- Post timing / frequency correlation

### Step 3: Voice Alignment Audit
Review a sample of content (10–20 pieces) against the brand voice file:
- Does it still sound like the current brand?
- Are banned words appearing?
- Is the tone consistent?
- Is the CTA approach consistent?

Flag content that's significantly off-brand for update or deletion.

### Step 4: Gap Analysis
Compare existing content against content pillars:
- Which pillars are overcrowded? (stop creating more here, or repurpose what exists)
- Which pillars are underserved? (prioritize these in the next quarter)
- Are there audience questions that no content addresses?

### Step 5: Action Classification

Classify every piece of content:
- **Keep:** On-brand, performing, no action needed
- **Update:** Good idea, but needs voice refresh, new data, or updated CTA
- **Repurpose:** High-performing, adapt to another platform or format
- **Rewrite:** Core topic is right, but execution is wrong
- **Archive/Delete:** Off-brand, outdated, or permanently underperforming

## Audit Output

```
CONTENT AUDIT: [Brand Name]
Platforms: 
Period covered: 
Total pieces reviewed: 

---

PERFORMANCE PATTERNS (if data available):
Top performing topics: 
Top performing formats: 
What high performers have in common: 
What underperformers have in common: 

VOICE ALIGNMENT:
Overall: [Strong / Some drift / Significant drift]
Issues found: 

GAP ANALYSIS:
Overcrowded pillars: 
Underserved pillars: 
Missing content types: 

ACTION LIST:
Keep: [X pieces]
Update: [list titles + what to change]
Repurpose: [list titles + suggested format]
Rewrite: [list titles + what to fix]
Archive/Delete: [list titles + reason]

STRATEGIC RECOMMENDATIONS:
1. 
2. 
3. 

NEXT 30 DAYS:
Priority actions based on audit findings:
- [ ] 
- [ ] 
- [ ] 
```

## Related Skills

- `content-strategist` — build new strategy based on audit findings
- `content-repurposer` — execute the repurposing list from the audit
- `content-editor` — execute the update list from the audit
- `editorial-calendar` — build the next quarter's calendar from gap analysis
