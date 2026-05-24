---
name: hook-writer
description: When the user wants to write or improve hooks for any content. Also use when the user says "write me some hooks," "help with my opening line," "I need a better hook," "hook options for this post," "opening line," "first line," "make this catchier," "the hook isn't working," or wants multiple hook options before committing to one.
---

# Hook Writer

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `hook-database.json`
- `content-examples.json`

You generate multiple strong hooks for any content type — so the user can choose the one that fits rather than settling for the first idea.

## Context Check

Read `.agents/brand-voice.md`. Hooks are the most brand-exposed single line of any content. Voice must be exact.

## What a Hook Actually Is

A hook is not a title. It's not a teaser. It's not a trick.

A hook is the first moment of contact between the content and the reader — and its only job is to earn the second moment.

On social: the line visible before "see more"
On email: the subject line
On video: the first 3 seconds
On a landing page: the headline

The hook decides whether the rest of the content gets read.

## Hook Types

Generate hooks across these types for any given topic:

### 1. The Bold Claim
A strong, direct assertion. Confident, not hedged.
"Most content strategies are expensive distractions."
"You don't have a content problem. You have a hook problem."

### 2. The Counterintuitive
Challenges what the audience already believes.
"Posting more content is why your account isn't growing."
"The best LinkedIn posts don't go viral. They just don't need to."

### 3. The Specific Story Opener
Drops the reader into a scene or moment.
"Six months ago I had 400 followers and was ready to quit."
"I charged half my rate for three years. One conversation changed that."

### 4. The Relatable Frustration
Names a pain the audience has felt but hasn't seen articulated.
"You spent three hours writing a post. It got 12 likes. You want to quit."
"Every content tip tells you what to do. Nobody tells you in what order."

### 5. The Data / Stat Hook
A number that surprises or reframes.
"93% of LinkedIn posts get fewer than 1,000 impressions."
"The average newsletter open rate dropped 40% in the last two years."
(Only use real, credible data. Flag if the stat needs verification.)

### 6. The Question
Only works if the question creates genuine tension. Not: "Have you ever wondered about X?"
Yes: "What if everything you've been told about content consistency is wrong?"

### 7. The Consequence
Stakes-forward. Makes the reader feel what happens if they don't keep reading.
"If you're writing content without this, you're creating for an audience of zero."
"This mistake cost me 6 months of traction. It might be costing you too."

### 8. The Direct Address
Speaks to the reader's specific identity or situation.
"If you've been posting for 6 months with no results, read this."
"This is for the founders who hate 'authentic content' advice."

## Hook Generation Process

1. Get the topic, content type, and platform
2. Identify the core insight or most surprising element of the piece
3. Generate 8–12 hooks across different types
4. Flag top 2–3 with rationale
5. Note if a hook is risky (might alienate part of the audience or require strong follow-through)

## Output Format

```
HOOKS: [Topic / content type]
Platform: 
Core insight: [The thing the hook is building toward]

---

OPTION 1 — [Type]
Hook: 
Note: [Why this works / what it requires]

OPTION 2 — [Type]
Hook: 
Note: 

[...8–12 options]

---

TOP PICKS:
#1: Option [X] — [Reason]
#2: Option [X] — [Reason]

A/B TEST PAIR: Options [X] and [Y]
[Why these are the two strongest to test against each other]
```

## Hook Quality Rules

Before delivering, check each hook:
- [ ] No banned words from brand voice
- [ ] Doesn't over-promise what the content can't deliver
- [ ] Doesn't start with "I" as the first word (LinkedIn-specific: weakens opening)
- [ ] Doesn't start with a question that can be answered "no" ("Have you ever wondered...")
- [ ] Sounds like how this brand talks, not like generic AI thought leadership

## Related Skills

- `linkedin-post-writer` — hooks for LinkedIn posts
- `newsletter-writer` — subject lines use the same hook principles
- `youtube-script-writer` — video hooks (first 3 seconds)
- `video-title-writer` — title hooks for YouTube
- `content-editor` — assess existing hooks against these standards
