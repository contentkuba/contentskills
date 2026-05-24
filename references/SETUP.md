# Setup Guide

## Recommended: Setup Wizard (10 minutes)

Open `setup-wizard.html` from the repo root in your browser. Claude runs a short interview — about 12 questions across 6 phases — and generates all 14 reference files pre-filled with your actual content.

**What it covers:**
- Identity and brand positioning
- Audience psychographics and their exact language
- Voice descriptors, banned words, and signature POV
- Content pillars with example angles
- Active platforms, posting frequency, and CTA patterns

At the end: one button generates a ZIP. Unzip it and drop the `references/shared/` folder into your repo root. Every skill immediately reads your voice.

---

## Manual Setup (if you prefer to fill in files directly)

Fill in the files in this order. Each builds on the previous.

### 1. Core identity — do these first

**`references/shared/voice.json`**
- `voice_is` and `voice_is_not` — 5 descriptors each
- `signature_pov` — the one paragraph that captures your core belief
- `voice_examples` — paste 2 real pieces of your best content + 1 that sounds wrong

**`references/shared/audience.json`**
The psychographic fields matter more than demographics:
- `internal_monologue` — what does your reader say to themselves when facing the problem you solve?
- `language_they_use` — exact phrases, not paraphrases
- `trust_objection` — what stops them trusting your content before they know you?

### 2. Writing rules

**`references/shared/writing-style.json`**
Describe what your writing actually looks like, not what you wish it looked like.

**`references/shared/preferred-banned-words.json`**
Open 5 of your best posts and pull the vocabulary you reach for naturally. Add your personal aversions to the banned list — the AI-cliché defaults are already there.

**`references/shared/dos-donts.json`**
Review the defaults — most apply universally. Add 2–3 brand-specific rules at the bottom of each list.

### 3. Content strategy

**`references/shared/content-pillars.json`**
Define 5–8 pillars. Each should connect to your audience's real problems and have at least 3 `example_angles` you could write tomorrow.

**`references/shared/brand-identity.json`**
- `offers` — every active offer with its specific CTA
- `positioning` — what category you compete in and how you're different
- `social_proof.notable_results` — 3 real, specific results

### 4. Platform configuration

**`references/shared/platform-settings.json`**
For each active platform, set `active: true` and fill in frequency, tone, and hashtag settings. Skip inactive platforms.

### 5. CTAs and content examples

**`references/shared/cta-style.json`**
List every live DM keyword trigger so skills never create conflicts. Paste your real CTAs verbatim.

**`references/shared/content-examples.json`**
The most important file for voice fidelity. Paste 10–15 real pieces of your best content across different formats. Fill in `what_works` for each.

### 6. Optional but high-value

**`references/shared/seo-keywords.json`** — only if you create SEO content or YouTube videos

**`references/shared/visual-language.json`** — only if you create video or carousel content

---

## Minimum viable setup

If you need to use skills immediately, fill in just these 4 files and everything works at a basic level:

1. `voice.json` — `voice_is`, `voice_is_not`, `signature_pov`, one `voice_examples` entry
2. `preferred-banned-words.json` — 10 preferred words + the default banned list
3. `audience.json` — `role`, `biggest_challenge`, `internal_monologue`, `language_they_use`
4. `content-pillars.json` — 3 pillars minimum

Upgrade to full setup within the first week as you use the skills and notice gaps.

---

## Keeping reference files current

Update them when:
- Your offer or positioning changes
- You develop new vocabulary or find new banned words
- A new keyword trigger goes live
- You add new content examples — do this regularly, it's the highest-leverage update

Skills pick up changes automatically on next use.
