---
name: brand-voice
description: When the user wants to define, document, or update their brand voice. Also use when the user says "set up my brand voice," "define my tone," "create a voice guide," "I want the AI to sound like me," "save my brand context," "update my brand profile," or starts a new project and needs to configure voice before creating content. This is the foundation skill — all other content skills read it first.
---

# Brand Voice

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `audience.json`
- `brand-identity.json`
- `dos-donts.json`
- `preferred-banned-words.json`

**Also load:**
- `platform-settings.json`

You help users define and document their brand voice so every piece of content they create with AI sounds consistent, human, and on-brand.

## Context Check

Before asking questions, check if `.agents/brand-voice.md` exists (or `.claude/brand-voice.md` as fallback). If it exists, read it and use that context. Only ask for information not already covered or specific to this task.

If no brand voice file exists, run the full setup interview below.

## Setup Interview

When starting fresh, collect the following through conversation — don't dump all questions at once. Ask in natural groups.

### Who They Are
- What's the brand/creator name?
- What do you do, and who do you do it for? (one sentence)
- What's your content's primary goal? (build audience / generate leads / establish authority / sell)

### Audience
- Who is your ideal reader/follower? Be specific. (role, industry, level, pain points)
- What does your audience already believe that you agree with?
- What does your audience believe that you want to challenge?

### Tone & Personality
- Pick 3–5 words that describe your voice (e.g. direct, warm, contrarian, nerdy, irreverent)
- Pick 3–5 words that describe what your voice is NOT (e.g. corporate, preachy, salesy, overly casual)
- Name 2–3 creators/writers whose style you admire. What specifically do you like about them?

### Writing Rules
- Do you use "I" or "we"?
- Do you use humor? What kind?
- Do you swear? Never / occasionally / freely?
- How do you feel about jargon in your space? Embrace it / explain it / avoid it?
- Long-form or short punchy sentences? Or a mix?
- Do you use bullet points and lists, or flowing prose, or both?
- Do you name and call out common bad advice, bad actors, or industry BS?

### Content
- What are your 3–5 core content pillars? (the topics you always come back to)
- What topics are off-limits?
- What's your signature POV — the one thing you believe that most people in your space don't?

### Platform Preferences
- Which platforms do you post on? (LinkedIn / Instagram / X / YouTube / newsletter / blog)
- Are there platform-specific tone variations? (e.g. more casual on X, more polished on LinkedIn)

### Examples
- Paste 2–3 examples of content you've written that sounds like "you at your best"
- Paste 1 example of content that sounds wrong — too AI, too corporate, too generic

### Banned Words & Phrases
Collect any words/phrases the user hates or considers red flags. Common defaults to include unless overridden:
- "Dive into" / "delve into"
- "Game-changer" / "game-changing"
- "At the end of the day"
- "Leverage" (as a verb)
- "Unlock"
- "Excited to share"
- "Thrilled to announce"
- "In today's fast-paced world"
- "Seamless"
- "Robust"

### CTAs
- What's your default CTA style? (soft / direct / question / engagement bait)
- What CTAs do you use most? What do you never want to say?

## Output: Brand Voice File

After collecting all information, generate a brand voice file and save it to `.agents/brand-voice.md`.

Structure the file as:

```markdown
# Brand Voice: [Brand Name]

## Identity
- Name: 
- One-liner: 
- Primary content goal: 

## Audience
- Who they are: 
- What they believe: 
- What we challenge: 

## Tone
- Voice is: [list]
- Voice is NOT: [list]
- Writing style: 

## Writing Rules
- Pronoun: I / we
- Humor: 
- Jargon: 
- Sentence style: 
- Lists vs prose: 
- Contrarian: yes/no — [approach]

## Content Pillars
1. 
2. 
3. 

## Signature POV
[One paragraph — the core belief that shapes all content]

## Platform Notes
- LinkedIn: 
- Instagram: 
- X/Twitter: 
- YouTube: 
- Newsletter: 

## Banned Words & Phrases
[list]

## CTA Style
- Default approach: 
- Preferred CTAs: 
- Never say: 

## Voice Examples
### Sounds Like Me
[example 1]
[example 2]

### Does NOT Sound Like Me
[example]
```

## Updating Brand Voice

If the user says "update my brand voice," "change my tone," or "add to my voice profile":
1. Read the existing `.agents/brand-voice.md`
2. Ask specifically what they want to change
3. Make the edit and save the updated file
4. Confirm what changed

## How Other Skills Use This

Every content skill in this repo reads `.agents/brand-voice.md` before writing. The brand voice file is not optional — it's what makes AI-generated content sound like *you* instead of like AI.

If another skill is invoked and no brand voice file exists, that skill should run this skill first before proceeding.

## Related Skills

- `audience-persona` — deeper audience profiling, read after brand-voice is set
- `content-strategist` — uses brand voice to build content strategy
- `content-editor` — uses brand voice as the quality bar for edits
