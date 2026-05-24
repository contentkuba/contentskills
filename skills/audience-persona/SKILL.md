---
name: audience-persona
description: When the user wants to define, document, or refine their target audience. Also use when the user says "who am I writing for," "define my audience," "create a persona," "who is my ideal reader," "ICP for content," "customer profile," or "I don't know my audience." Run this after brand-voice is set. All platform writer skills use the output.
---

# Audience Persona

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `audience.json`
- `voice.json`
- `brand-identity.json`

**Also load:**
- `content-pillars.json`

You help users build a sharp, usable audience persona that informs every piece of content they create — not a generic demographic profile, but a psychographic portrait of the person they're actually trying to reach.

## Context Check

Check for `.agents/brand-voice.md` first and read it. Then check for `.agents/audience-persona.md`. If persona already exists, ask if they want to update it or create a new segment.

## The Problem with Generic Personas

Most audience personas are useless: "Marketing Mary, 35, likes coffee, uses LinkedIn." Avoid this. A content persona answers:
- What does this person *believe* that drives their decisions?
- What are they *afraid* of?
- What do they *want* to be true?
- Where do they get *stuck*?
- What makes them *roll their eyes*?

## Persona Interview

Collect through conversation, not a form dump.

### The Person
- Job title / role
- Industry
- Company size / type (if B2B) or life situation (if B2C)
- Experience level (junior / mid / senior / founder / executive)
- Where they hang out online (LinkedIn, Reddit, X, YouTube, newsletters)

### Their World
- What's their biggest professional/personal challenge right now?
- What keeps them up at night?
- What do they wish they were better at?
- What have they already tried that hasn't worked?
- What are they embarrassed to admit they don't know?

### Their Beliefs
- What do they currently believe about [your topic area]?
- What misconception do they hold that you want to correct?
- What do they know is true but struggle to act on?
- What do they think they need vs. what do they actually need?

### Their Content Behavior
- What kind of content do they actually engage with? (listicles, long essays, stories, data, hot takes)
- What makes them stop scrolling?
- What makes them share something?
- What makes them unfollow someone?
- What content do they consume but never admit to? (guilty pleasures)

### Their Relationship to You
- At what stage of awareness do they find you? (problem aware / solution aware / brand aware)
- What objection do they have before trusting your content?
- What would make them a loyal follower vs. a one-time reader?

### Their Language
- What exact words do they use to describe their problems? (quote-level specificity)
- What words or phrases do they hate hearing from people in your space?
- What's their private internal monologue when they face the problem you address?

## Output: Audience Persona File

Save to `.agents/audience-persona.md`. If multiple segments, create separate sections.

```markdown
# Audience Persona: [Brand Name]

## Primary Persona: [Name/Label]

### Who They Are
- Role: 
- Industry: 
- Experience: 
- Online: 

### Their World
- Biggest challenge: 
- What keeps them up: 
- What they've tried: 
- Embarrassing gap: 

### Their Beliefs
- Currently believes: 
- Misconception to correct: 
- Knows but doesn't act on: 

### Content Behavior
- Engages with: 
- Stops scrolling for: 
- Shares when: 
- Unfollows when: 

### Their Language
- Describes their problem as: 
- Hates hearing: 
- Internal monologue: 

### Relationship to Us
- Awareness stage: 
- Objection before trusting: 
- What makes them loyal: 

## Secondary Persona (if applicable): [Name/Label]
[same structure]
```

## Using the Persona in Content

When other skills run, the audience persona informs:
- **Hook writing** — speaks to their exact internal monologue
- **Content pillars** — addresses their real problems, not assumed ones
- **Tone** — matches their sophistication and communication style
- **CTAs** — respects their awareness stage and trust level

## Related Skills

- `brand-voice` — must be set before or alongside audience persona
- `content-brief` — uses persona to define content angle and intent
- `content-strategist` — uses persona to build pillars and calendar
- `hook-writer` — uses persona language for scroll-stopping hooks
