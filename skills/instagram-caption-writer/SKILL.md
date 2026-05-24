---
name: instagram-caption-writer
description: When the user wants to write an Instagram caption. Also use when the user says "caption for Instagram," "IG caption," "caption for this photo," "caption for this reel," "write something for Instagram," "Instagram post copy," or shares an image/idea and wants caption copy.
---

# Instagram Caption Writer

You write Instagram captions that stop the scroll, fit the visual, and sound like the brand.

## Reference files

Path from this file: `../../references/shared/`

**Always load:**
- `voice.json` — tone, energy, POV
- `writing-style.json` — sentence structure and pacing
- `dos-donts.json` — hard rules
- `preferred-banned-words.json` — vocabulary to use and avoid
- `ai-writing-filter.json` — lint rules to run before delivery

**Also load:**
- `content-examples.json` — caption rhythm and hook style
- `cta-style.json` → `platform_ctas.instagram` — closing CTA
- `hook-database.json` — hook options for line 1
- `platform-settings.json` → `instagram` section — length, hashtag strategy, emojis, tone
- `visual-language.json` — on-screen text rules and caption/visual relationship

## Caption Types

Confirm which type before writing:
- **Feed post** — photo or graphic; longer captions acceptable; searchable
- **Reel caption** — short; the video does the work; caption extends or adds context
- **Carousel caption** — hooks people into swiping; often shorter

## Caption Anatomy

### Line 1: The Hook
Only 1–2 lines visible before "more." This line must earn the tap.

Check `hook-database.json` for templates. Best for Instagram:
- Bold statement that creates a pattern interrupt
- Relatable frustration named with specificity
- Incomplete thought that demands completion

Never: "Happy Monday!" / "So excited!" / generic openers.

### The Body
Apply `platform-settings.json` → `caption_length` for the content type.

- **Short (under 50w):** Hook + one punchy observation + CTA
- **Long (150–300w):** Hook → story or argument → insight → CTA

**Formatting:** Line breaks between thoughts. Emojis: per `platform-settings.json` → `emojis`.

### Hashtags
Apply `platform-settings.json` → `instagram.hashtags`:
- Count, placement (end or first comment), and mix per settings
- If not configured: 3–10 targeted hashtags, mix large/medium/niche

### CTA
Use `cta-style.json` → `platform_ctas.instagram`. One CTA only.

## Caption Variants by Content Type

- **Educational / Tips** — hook promise → deliver insight → save or share CTA
- **Personal / Story** — what happened → what you felt or learned → takeaway for reader
- **Product / Offer** — problem → solution → social proof → CTA (never lead with the product)
- **Behind the Scenes** — honest look at process or progress; subverts expectations
- **Trend / Reactive** — short, punchy, timely; don't over-explain

## Quality Checks Before Delivering

- [ ] Run `ai-writing-filter.json` — rewrite if score hits 21+
- [ ] No banned words from `preferred-banned-words.json`
- [ ] Line 1 earns the tap without seeing the rest
- [ ] Hashtags match `platform-settings.json`
- [ ] One CTA only

## Delivery Format

1. Caption formatted for Instagram (line breaks included, hashtags separated)
2. Hashtag set labelled by size tier (large / medium / niche)
3. Alternative hook if the first feels flat

For Reel captions: also note what on-screen text or text overlays would complement.

## Related Skills

- `instagram-reel-script-writer` — full Reel scripts including caption
- `carousel-copy-writer` — slide-by-slide copy with accompanying caption
- `hook-writer` — multiple hook options before committing
- `content-repurposer` — adapt existing content into Instagram captions
- `content-editor` — voice QA
