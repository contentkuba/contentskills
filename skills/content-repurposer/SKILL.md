---
name: content-repurposer
description: When the user wants to repurpose existing content into other formats. Also use when the user says "repurpose this," "turn this into X," "make more content from this," "adapt this for LinkedIn," "turn this blog post into a carousel," "I want to get more out of this piece," "content from this podcast/video/article," or shares content and wants it adapted to another platform or format.
---

# Content Repurposer

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `writing-style.json`
- `dos-donts.json`
- `preferred-banned-words.json`
- `ai-writing-filter.json`

**Also load:**
- `content-pillars.json`
- `platform-settings.json`

You take one piece of content and extract maximum value from it — turning a single source into multiple platform-specific pieces without copy-pasting or watering it down.

## Context Check

Read `.agents/brand-voice.md`. Repurposed content must go through the brand voice filter — platform adaptation isn't just cutting and pasting, it's translating.

## The Repurposing Principle

Repurposing is NOT:
- Copying a blog post into a LinkedIn post
- Sharing a link with a generic caption
- Splitting a post into multiple smaller posts

Repurposing IS:
- Identifying the core insight and re-expressing it for a different format and platform context
- Finding the 3 quotes worth pulling from a podcast
- Turning the framework in an article into a carousel visual
- Extracting the story buried in a report and making it a LinkedIn narrative

## Source Content Types

The skill handles repurposing from any starting point:

- **Blog post / article** — highest leverage; most ideas, most repurposable
- **LinkedIn post** — expand into blog, compress into X thread, convert to carousel
- **Newsletter issue** — extract the best insight for social, expand for blog
- **Podcast episode** — transcript-based; quotes, stories, frameworks
- **Video / YouTube script** — companion blog, clip scripts, quote pulls
- **Talk / presentation** — each slide = a social post; key quotes = newsletter
- **Raw notes / voice memo** — identify the idea worth developing

## Repurposing Map (Standard)

When given a source, generate a full repurposing map:

```
SOURCE: [Title / type]
Core insight: [The one idea worth spreading]

REPURPOSING MAP:
→ LinkedIn post: [angle — story / insight / contrarian]
→ Instagram carousel: [framework / tips from the piece]
→ Instagram Reel: [hook — the most surprising line]
→ X thread: [compressed argument or numbered list]
→ Newsletter section: [the insight + application for subscribers]
→ Blog post: [expanded treatment if source was short-form]
→ Quote graphic: [pull quote for visual]
→ YouTube short hook: [30-second version of the core idea]
```

Then ask: which formats does the user want adapted? Or produce all if requested.

## Format Adaptation Rules

Each format has its own translation logic:

**Blog → LinkedIn**
Extract the one strongest insight (not the whole article). Rewrite from scratch with LinkedIn formatting (line breaks, no walls). The blog link goes at the end, not the beginning.

**Blog → Carousel**
Identify the framework or list structure. Each major point = one slide. Compress to 6–10 words per slide.

**Blog → Newsletter**
The intro becomes the hook. Pull the most surprising fact or story. Compress the body to the key insight + practical takeaway.

**Podcast → Social**
Pull the 3 best quotes. For each, write a post around the quote (the quote is supporting evidence, not the whole post).

**Video → Blog**
Transcript → remove filler → restructure with H2s → add depth where the video glossed over.

**LinkedIn → Instagram**
LinkedIn voice is slightly more formal. Translate to Instagram: warmer, more visual language, shorter, more emotive hook.

**Long → Short**
Find the sharpest sentence in the piece. Build the short-form version around that one line.

## Quality Check

Before delivering any repurposed piece, verify:
- [ ] It doesn't read like a copy-paste
- [ ] The format matches the platform's norms
- [ ] The hook is rewritten, not taken directly from source
- [ ] Banned words from brand voice are removed
- [ ] The CTA fits the platform

## Output

When given a source, deliver:

1. The repurposing map (all possible formats)
2. Ask which formats to develop, or develop all if specified
3. Each developed piece, fully formatted for its platform
4. Note any pieces that don't work well for this source content (and why)

## Related Skills

- `linkedin-post-writer` — final polish for LinkedIn adaptations
- `carousel-copy-writer` — slide-by-slide structure for carousel adaptations
- `instagram-caption-writer` — Instagram-specific caption treatment
- `newsletter-writer` — newsletter section development
- `content-editor` — QA all repurposed pieces before publishing
