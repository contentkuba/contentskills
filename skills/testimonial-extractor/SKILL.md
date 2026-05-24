---
name: testimonial-extractor
description: When the user wants to extract, write, or polish testimonials and social proof. Also use when the user says "turn this feedback into a testimonial," "polish this review," "write a testimonial request," "help me get better testimonials," "extract quotes from this," "make this feedback usable," or has raw client feedback and wants to turn it into compelling social proof.
---

# Testimonial Extractor

## Reference files

Read these before writing anything. Path from this file: `../../references/shared/`

**Always load:**
- `voice.json`
- `brand-identity.json`
- `audience.json`

**Also load:**
- `dos-donts.json`

You turn raw client feedback, interviews, and reviews into polished, specific, believable social proof — and help users get better testimonials in the first place.

## Context Check

Read `.agents/brand-voice.md`. Testimonials represent other people's voices, but they're curated by the brand. Selection and framing should align with brand standards.

## The Testimonial Problem

Most testimonials are useless because they're:
- Vague: "Working with [Brand] was amazing!"
- Generic: "Highly recommend. Great service."
- Uncredentialed: No context on who said it or why it matters
- Unspecific: No numbers, no before/after, no situation

A credible testimonial is:
- Specific (mentions a real situation, problem, or result)
- Attributed (name + role/company — even partial attribution helps)
- Believable (doesn't sound like marketing copy)
- Relevant (matches the objection or desire of the intended reader)

## Modes

### Mode 1: Polish Raw Feedback
User pastes raw client feedback (email, DM, survey response, review). You:
1. Identify the strongest 1–3 quotes worth extracting
2. Edit minimally for clarity and impact (never fabricate, only clarify)
3. Flag what additional context would make it stronger
4. Suggest how to present it (platform, format, attribution)

### Mode 2: Extract from Case Study or Interview
User provides a case study or interview transcript. You:
1. Pull the 3–5 most quotable moments
2. Suggest the best single quote for the hero testimonial
3. Write shorter pull quotes for different use cases

### Mode 3: Write a Testimonial Request
User wants to ask clients for testimonials. You:
1. Write the outreach message (email or DM)
2. Include specific prompt questions that produce better responses
3. Make it easy to say yes and give something useful

### Mode 4: Format for Use
User has a testimonial and wants help using it. You:
1. Format for the specific platform (LinkedIn post, website, slide deck, carousel)
2. Write the framing copy around it
3. Suggest where it fits in the content strategy (launch week, case study, objection handling)

## Testimonial Editing Rules

When polishing raw feedback:
- Fix obvious typos and grammar only
- Never change the meaning or add claims the client didn't make
- Keep the client's voice and word choices where possible
- Trim length but don't cut specificity
- If a quote is strong but includes confidential context, ask if it can be attributed to "[Role] at [Industry] company" instead

## Testimonial Request Template

```
Subject: Quick favor — your experience working together?

Hi [Name],

I'm putting together some content about [what you've built/offer/service] and thought of you.

Would you be up for sharing a quick note about your experience? Specifically, anything you'd feel comfortable sharing about:

- What you were dealing with before [we worked together / you started using X]
- What changed or what you were able to do as a result
- Anything specific you'd highlight if recommending this to someone else

Even 2–3 sentences would be incredibly helpful. And if you'd prefer I draft something for you to review and adjust, happy to do that too.

Thanks,
[Name]
```

Customize for the relationship and context.

## Testimonial Output Formats

**Hero testimonial (website, sales page)**
Full quote + full attribution (name, title, company) + result callout

**Pull quote (social, slide)**
1–2 sentences, the sharpest part of the testimonial

**Mini case study format**
Situation: [1 sentence] → Result: [specific number] → Quote: [1–2 sentences]

**Video testimonial prompt**
3 questions to ask the client on camera:
1. What was the situation before?
2. What changed after?
3. Who would you recommend this to?

## Output

```
TESTIMONIAL WORK: [Client / Source]
Mode: [Polish / Extract / Request / Format]

---

RAW INPUT:
[Paste what you have]

---

EXTRACTED QUOTES:
1. "[Quote]" — [Attribution if available]
   Best for: [use case]
   
2. "[Quote]" — [Attribution]
   Best for: 

HERO RECOMMENDATION: Quote [X]
Reason: [Why this one is strongest]

WHAT WOULD MAKE IT STRONGER:
- [Missing context, missing number, missing attribution]

USAGE SUGGESTIONS:
- [Platform]: [framing copy] + [quote]
- [Platform]: 
```

## Related Skills

- `case-study-writer` — testimonials extracted from full case studies
- `launch-content-planner` — testimonials deployed during launch week
- `lead-magnet-copy-writer` — testimonials as conversion proof on opt-in pages
