# Reference Map

All shared reference files live in `references/shared/`. Each skill loads the files listed below before writing anything. The path from any skill is `../../references/shared/[filename]`.

Skills with skill-specific reference files (like `instagram-reel-script-writer`) also load from their own `references/` subfolder.

---

## Shared Reference Files

| File | What It Contains |
|---|---|
| `voice.json` | Brand voice, tone, energy, personality, signature POV |
| `writing-style.json` | Sentence length, structure, storytelling arc, pacing |
| `dos-donts.json` | Hard rules for all content |
| `preferred-banned-words.json` | Vocabulary to use and avoid |
| `ai-writing-filter.json` | AI signal lint rules — run before every delivery |
| `audience.json` | Psychographic audience profile |
| `brand-identity.json` | Brand positioning, offers, social proof |
| `content-pillars.json` | Topic areas and pillar mix rules |
| `content-examples.json` | Real examples of best-performing content |
| `cta-style.json` | CTA philosophy, active keyword triggers, platform CTAs |
| `platform-settings.json` | Per-platform format rules, frequency, hashtag strategy |
| `hook-database.json` | 50 hook templates to adapt |
| `visual-language.json` | Video/image setups, B-roll, on-screen text, design notes |
| `seo-keywords.json` | Keyword strategy for SEO, blog, and YouTube |

---

## Reference Load Map Per Skill

### Foundation Skills
| Skill | Loads |
|---|---|
| `brand-voice` | voice · writing-style · audience · brand-identity · dos-donts · preferred-banned-words · platform-settings |
| `audience-persona` | audience · voice · brand-identity · content-pillars |

### Research & Strategy Skills
| Skill | Loads |
|---|---|
| `content-research` | voice · audience · content-pillars · brand-identity |
| `content-brief` | voice · writing-style · audience · content-pillars · seo-keywords |
| `content-strategist` | voice · audience · brand-identity · content-pillars · platform-settings · content-examples |
| `editorial-calendar` | content-pillars · platform-settings · content-examples · cta-style |
| `content-audit` | voice · content-pillars · platform-settings · preferred-banned-words |
| `trend-jacking` | voice · writing-style · dos-donts · preferred-banned-words · cta-style · ai-writing-filter |

### Platform Writer Skills
| Skill | Loads |
|---|---|
| `linkedin-post-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · content-examples · cta-style · hook-database · platform-settings[linkedin] · ai-writing-filter |
| `instagram-caption-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-examples · cta-style · hook-database · platform-settings[instagram] · visual-language · ai-writing-filter |
| `instagram-reel-script-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · content-examples · cta-style · hook-database · visual-language · ai-writing-filter + skill-specific references |
| `carousel-copy-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · content-examples · cta-style · hook-database · visual-language · platform-settings · ai-writing-filter |
| `x-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-examples · cta-style · hook-database · platform-settings[x_twitter] · ai-writing-filter |
| `newsletter-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · content-examples · cta-style · platform-settings[newsletter] · brand-identity · ai-writing-filter |

### Long-Form & Video Skills
| Skill | Loads |
|---|---|
| `blog-post-writer` | voice · writing-style · dos-donts · preferred-banned-words · audience · content-pillars · cta-style · platform-settings[blog] · ai-writing-filter |
| `seo-content-writer` | voice · writing-style · dos-donts · preferred-banned-words · audience · seo-keywords · cta-style · platform-settings[blog] · ai-writing-filter |
| `infographic-designer` | voice · content-pillars · audience · visual-language · brand-identity |
| `youtube-script-writer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · cta-style · hook-database · platform-settings[youtube] · visual-language · ai-writing-filter |
| `youtube-description-writer` | voice · seo-keywords · cta-style · platform-settings[youtube] · brand-identity |
| `video-title-writer` | voice · hook-database · seo-keywords · platform-settings[youtube] · dos-donts |

### Workflow & Quality Skills
| Skill | Loads |
|---|---|
| `content-repurposer` | voice · writing-style · dos-donts · preferred-banned-words · content-pillars · platform-settings · ai-writing-filter |
| `content-editor` | voice · writing-style · dos-donts · preferred-banned-words · ai-writing-filter · content-examples |

### Distribution & Growth Skills
| Skill | Loads |
|---|---|
| `content-distribution` | voice · audience · content-pillars · platform-settings · brand-identity |
| `podcast-pitch-writer` | voice · brand-identity · audience · content-pillars |
| `comment-writer` | voice · writing-style · dos-donts · preferred-banned-words · ai-writing-filter |
| `launch-content-planner` | voice · audience · brand-identity · content-pillars · platform-settings · cta-style |

### Trust & Conversion Skills
| Skill | Loads |
|---|---|
| `case-study-writer` | voice · writing-style · dos-donts · preferred-banned-words · brand-identity · ai-writing-filter |
| `testimonial-extractor` | voice · brand-identity · audience · dos-donts |
| `lead-magnet-copy-writer` | voice · writing-style · dos-donts · preferred-banned-words · audience · brand-identity · cta-style · ai-writing-filter |

### Utility Skills
| Skill | Loads |
|---|---|
| `hook-writer` | voice · writing-style · dos-donts · preferred-banned-words · hook-database · content-examples · ai-writing-filter |
| `cta-writer` | voice · cta-style · dos-donts · preferred-banned-words · platform-settings |

---

## Skill-Specific Reference Files

The `instagram-reel-script-writer` skill includes its own `references/` subfolder with video-specific versions of several files already populated from the creator's existing Reel content. All other skills read from `references/shared/` only.

As you add more voice-specific examples for other skills (e.g., a LinkedIn-specific hook database, a carousel-specific style guide), add them to the relevant skill's own `references/` subfolder and update this map.
