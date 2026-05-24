# Content Skills for AI Agents

A collection of AI agent skills for content marketing. Built for creators, founders, and content teams who want AI coding agents to help with writing, strategy, distribution, and everything in between.

Works with Claude Code, Cursor, Windsurf, and any agent that supports the [Agent Skills spec](https://agentskills.io).

## How Skills Work Together

Every skill reads `brand-voice` first. That's what makes content sound like *you* instead of like AI.

```
                         ┌─────────────────┐
                         │   brand-voice   │
                         │  (all read me)  │
                         └────────┬────────┘
                                  │
         ┌───────────┬────────────┼────────────┬──────────────┐
         ▼           ▼            ▼            ▼              ▼
    Platform      Long-form    Strategy     Workflow       Trust &
    Writers       & Video      & Planning   & Quality      Conversion
   ──────────    ──────────   ──────────   ──────────     ──────────
   linkedin      blog-post    strategist   repurposer     case-study
   instagram-    seo-content  editorial-   editor         testimonial
   caption       infographic  calendar     auditor        lead-magnet
   reel-script   youtube-     launch-      distributor
   carousel      script       planner      podcast-pitch
   x-writer      youtube-     trend-       comment
   newsletter    description  jacking
                 video-title  audience-
                 content-     persona
                 brief        content-
                 content-     research
                 research
```

## Available Skills

### Foundation
| Skill | Description |
|---|---|
| [brand-voice](skills/brand-voice) | Define and document your brand voice — read by all other skills first |
| [audience-persona](skills/audience-persona) | Build a psychographic portrait of your ideal reader |

### Research & Strategy
| Skill | Description |
|---|---|
| [content-research](skills/content-research) | Find angles, data, and competitive gaps before writing |
| [content-brief](skills/content-brief) | Plan a piece strategically before drafting |
| [content-strategist](skills/content-strategist) | Build a content strategy from goal to execution |
| [editorial-calendar](skills/editorial-calendar) | Turn strategy into a concrete, realistic posting schedule |
| [content-audit](skills/content-audit) | Assess what's working, what to update, what to kill |

### Platform Writers
| Skill | Description |
|---|---|
| [linkedin-post-writer](skills/linkedin-post-writer) | LinkedIn posts that sound human and earn engagement |
| [instagram-caption-writer](skills/instagram-caption-writer) | Feed, Reel, and carousel captions for Instagram |
| [instagram-reel-script-writer](skills/instagram-reel-script-writer) | Full Reel scripts with hook, retention, and CTA |
| [carousel-copy-writer](skills/carousel-copy-writer) | Slide-by-slide carousel copy for LinkedIn and Instagram |
| [x-writer](skills/x-writer) | Posts and threads for X, Threads, and Notes |
| [newsletter-writer](skills/newsletter-writer) | Newsletter issues in multiple formats |

### Long-Form Content
| Skill | Description |
|---|---|
| [blog-post-writer](skills/blog-post-writer) | Thought leadership articles worth reading |
| [seo-content-writer](skills/seo-content-writer) | Search-optimized content that ranks and converts |
| [infographic-designer](skills/infographic-designer) | Infographic concept, copy, and designer brief |

### Video
| Skill | Description |
|---|---|
| [youtube-script-writer](skills/youtube-script-writer) | Full YouTube video scripts built for retention |
| [youtube-description-writer](skills/youtube-description-writer) | Descriptions that rank and convert |
| [video-title-writer](skills/video-title-writer) | Titles and thumbnail copy that earn the click |

### Workflow & Quality
| Skill | Description |
|---|---|
| [content-repurposer](skills/content-repurposer) | Turn one piece of content into many |
| [content-editor](skills/content-editor) | QA drafts against brand voice |
| [trend-jacking](skills/trend-jacking) | On-brand reactive content for timely moments |

### Distribution & Growth
| Skill | Description |
|---|---|
| [content-distribution](skills/content-distribution) | Get content in front of the right people |
| [podcast-pitch-writer](skills/podcast-pitch-writer) | Guest pitches that get replies |
| [comment-writer](skills/comment-writer) | Strategic comments that build visibility |
| [launch-content-planner](skills/launch-content-planner) | Full content sequence for launches |

### Trust & Conversion
| Skill | Description |
|---|---|
| [case-study-writer](skills/case-study-writer) | Client stories built on specificity |
| [testimonial-extractor](skills/testimonial-extractor) | Turn raw feedback into compelling social proof |
| [lead-magnet-copy-writer](skills/lead-magnet-copy-writer) | Landing page, opt-in, and delivery copy |

### Utility
| Skill | Description |
|---|---|
| [hook-writer](skills/hook-writer) | Multiple hook options for any content type |
| [cta-writer](skills/cta-writer) | CTAs that feel natural and get clicked |

## Installation

### Step 1 — Get the repo

```bash
git clone https://github.com/[your-username]/contentskills.git
```

Or install via Claude Code:

```bash
/plugin marketplace add [your-username]/contentskills
/plugin install content-skills
```

### Step 2 — Set up your brand voice (10 minutes)

Open `setup-wizard.html` in your browser. Claude interviews you conversationally — ~12 questions across 6 phases — then generates all 14 reference files pre-filled with your voice, audience, and content strategy. Download the ZIP, drop the contents into `references/shared/`. Done.

> **Manual setup:** If you prefer to fill in the JSON files directly, see [`references/SETUP.md`](references/SETUP.md).

### Step 3 — Use the skills

```
"Write a LinkedIn post about why I stopped posting every day"
→ linkedin-post-writer reads your voice, audience, and pillars automatically

"Turn this blog post into a carousel, a newsletter section, and a Reel hook"
→ content-repurposer adapts everything to your voice and platform settings

"Build me a 90-day content strategy"
→ content-strategist uses your pillars, audience, and platform preferences

"I'm launching next month — plan my content"
→ launch-content-planner uses your brand identity and active offers
```

## Usage

Start by setting up your brand voice — all other skills depend on it:

```
"Set up my brand voice"
→ Uses brand-voice skill — creates .agents/brand-voice.md

"Write a LinkedIn post about why I stopped posting every day"
→ Uses linkedin-post-writer skill (reads brand-voice first)

"Turn this blog post into a carousel, a newsletter section, and a Reel hook"
→ Uses content-repurposer skill

"Build me a 90-day content strategy"
→ Uses content-strategist + editorial-calendar skills

"I'm launching next month — plan my content"
→ Uses launch-content-planner skill
```

## The System

These skills are designed to work as a pipeline:

**Strategy pipeline:**
`brand-voice` → `audience-persona` → `content-strategist` → `editorial-calendar`

**Creation pipeline:**
`content-research` → `content-brief` → [platform writer] → `content-editor`

**Distribution pipeline:**
[any content] → `content-repurposer` → `content-distribution`

**Launch pipeline:**
`launch-content-planner` → [platform writers] → `case-study-writer` → `testimonial-extractor`

## Contributing

PRs and issues welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

[MIT](LICENSE)
