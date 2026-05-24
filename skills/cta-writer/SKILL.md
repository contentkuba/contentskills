---
name: cta-writer
description: When the user wants to write or improve a call-to-action. Also use when the user says "write a CTA," "improve my CTA," "what should my CTA be," "how do I end this," "the close is weak," "CTA options," "what should I ask people to do," or has content where the ending or ask isn't working.
---

# CTA Writer

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `cta-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`

**Also load:**
- `platform-settings.json`

You write calls-to-action that feel natural and get clicked — not desperate, not generic, not an afterthought.

## Context Check

Read `.agents/brand-voice.md`. The CTA style and approach should be defined in the voice file. Apply it exactly — some brands never use hard CTAs; some always do.

## The CTA Problem

Most CTAs fail because they're:
- Generic ("Follow me for more content like this")
- Demanding ("Share this NOW")
- Mismatched to the content (a personal story ending with "Buy my course")
- Buried in a paragraph
- Multiple CTAs competing with each other (pick one)

A good CTA:
- Asks for one thing
- Feels like the natural next step after the content
- Matches the relationship level (don't ask for a purchase after meeting someone)
- Gives the reader a reason to act

## CTA Ladder

Different content builds different levels of trust. Match the CTA to where the relationship is:

**Awareness content** (new audience)
→ Save / Share / Follow / Subscribe

**Consideration content** (warm audience)
→ Reply / Comment / Download / Read more

**Conversion content** (ready audience)
→ Book / Buy / Join / Apply

Never skip rungs. A cold audience post shouldn't end with "Book a call."

## CTA Types by Platform

### LinkedIn
- Engagement: "What's your experience with this? Comment below."
- Follow: "Follow for [frequency] posts on [topic]."
- Soft: "Save this for the next time you [relevant situation]."
- Traffic: "I wrote more about this in [article/newsletter] — link in comments."

### Instagram
- Save: "Save this for when you need it."
- Share: "Send this to someone who [relevant situation]."
- Comment: "Drop a [emoji] if this resonated."
- Profile: "More like this on my profile."

### Newsletter
- Reply: "Hit reply and tell me [specific question] — I read every response."
- Share: "If this was useful, forward it to one person who'd get something from it."
- Click: "[Link] — [what's there and why it's worth the click]"
- Next issue tease: "Next week: [specific, compelling topic]."

### YouTube / Video
- Subscribe: "Subscribe — I post [frequency] on [topic]."
- Next video: "If you want to go deeper on [related topic], I made a video — it's right here."
- Comment: "Tell me in the comments: [specific question that invites real answers]"

### Landing Pages / Emails
- Button text: Never "Submit" or "Click here." Always "Get [specific thing]" / "Start [specific outcome]" / "Yes, [specific desire]"
- Urgency (use carefully): Only when genuine. "Offer ends [date]" when it actually does.

## CTA Generation

When generating CTA options for a piece of content, ask:
- What platform is this for?
- What's the one action that would be most valuable for the business right now?
- What's the relationship level? (cold / warm / hot)
- What's the tone of the content? (light / serious / educational / personal)

Then generate 5–7 CTA options across types (soft / engagement / follow / traffic / conversion), with a recommendation.

## Output Format

```
CTA OPTIONS: [Content type / platform]
Audience relationship: [cold / warm / hot]
Business goal: 

---

OPTION 1 — [Type: soft / engagement / follow / traffic / conversion]
CTA: 
Tone: 

OPTION 2 — [Type]
CTA: 
Tone: 

[...5–7 options]

---

RECOMMENDED: Option [X]
Reason: [Why it fits this piece, this audience, this goal]

WHAT TO AVOID HERE:
[Any CTA types that would feel wrong for this specific piece — and why]
```

## Related Skills

- `hook-writer` — same principle, opposite end of the piece
- `content-editor` — CTA assessment is part of every edit
- `lead-magnet-copy-writer` — CTA button text for landing pages
- `newsletter-writer` — newsletter-specific CTA options
