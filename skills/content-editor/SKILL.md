---
name: content-editor
description: When the user wants to edit, improve, or QA existing content. Also use when the user says "edit this," "improve this draft," "review this," "make this sound better," "does this sound like me," "clean this up," "is this good," "fix this post," "run this through the filter," or shares a draft and wants feedback or a rewrite.
---

# Content Editor

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `content-examples.json`

You edit content drafts against the brand voice — fixing what's off, sharpening what's weak, and leaving alone what's already working.

## Context Check

Read `.agents/brand-voice.md` before editing anything. The brand voice file is the editing standard. Without it, editing is just preference. Run `brand-voice` first if the file doesn't exist.

## What Good Editing Is Not

Not: making it longer
Not: making it more "professional"
Not: adding caveats and qualifications
Not: rewording things that already work just to feel useful

Good editing removes what weakens the piece and sharpens what's already there.

## Editorial Framework

Run every draft through these checks, in order:

### 1. Voice Check
Does this sound like the brand?
- Read aloud. Does it sound like how this person talks?
- Compare against example posts in the brand voice file
- Flag: anything that sounds AI-written, corporate, or generic

### 2. Banned Words Audit
Scan for every word on the banned list in the brand voice file.
Flag each instance. Suggest a replacement or restructure.

### 3. Hook Assessment
Is the first line doing its job?
- For social: does it earn the "read more" / stop the scroll?
- For email: would you open this if a friend sent it?
- For blog: does it make you want the second paragraph?

Rate the hook: Strong / Needs work / Rewrite entirely
If "Needs work" or "Rewrite," provide 2 alternative hooks.

### 4. Structural Check
Does the piece have a clear arc?
- Is there a clear progression from opening to close?
- Does every paragraph / section add something new?
- Are there sections that could be cut without losing anything?

Flag any section that:
- Repeats something already said
- Adds padding without value
- Could be a sentence instead of a paragraph

### 5. Clarity Check
Is every sentence saying something?
Flag:
- Filler phrases ("It's worth noting that..." / "At the end of the day..." / "Basically...")
- Passive voice where active is sharper
- Overly qualified statements that hedge the point to death
- Jargon used without payoff

### 6. Landing Check
Does the close land?
- Does the final line stick?
- Is the CTA clear, singular, and appropriate for the platform?
- Does it feel complete, not just ended?

### 7. Platform Fit
Is the format right for the platform?
- LinkedIn: line breaks, no walls, CTA at end
- Instagram: hook above fold, hashtags at end
- Newsletter: short paragraphs, one idea per section
- Blog: H2 structure, no keyword stuffing, CTA

## Editing Output Format

Deliver edits in two parts:

**Part 1: Editorial Report**
```
EDITORIAL REPORT: [Content title/type]

Voice: [On brand / Off in places / Significantly off]
Hook: [Strong / Needs work / Rewrite]
Structure: [Clean / Has issues — see notes]
Clarity: [Sharp / Wordy — see flags]
Close: [Strong / Weak — see notes]
Platform fit: [Good / Issues — see notes]

FLAGS:
- Line X: [issue] → [suggested fix]
- Line X: [banned word] → [replacement]
- [Section]: [structural issue]

OVERALL: [1–2 sentences on biggest priority]
```

**Part 2: Edited Draft**
The full revised version, with changes made. Use the report flags as the editing guide. Don't over-edit — preserve the original voice where it's working.

## Light Edit vs. Full Rewrite

Ask or infer which the user needs:

**Light edit:** Fix specific issues (banned words, one weak section, tighten the close). Preserve structure and most of the copy.

**Full rewrite:** The voice or structure is significantly off. Take the core idea and rewrite from scratch, using the brand voice as the new foundation.

For a full rewrite: confirm before doing it, as it's a significant change.

## Related Skills

- `brand-voice` — the standard for all edits
- `hook-writer` — when the hook needs replacement options
- `cta-writer` — when the CTA specifically needs reworking
- `content-repurposer` — sometimes "edit this for Instagram" means adaptation, not editing
