---
name: serp-feature-optimization
description: Optimize eligible content for observed SERP features by matching the information format users are currently being shown, without fixed snippet-length rules or ranking guarantees.
---

# Serp Feature Optimization

## Purpose
Optimize eligible content for observed SERP features by matching the information format users are currently being shown, without fixed snippet-length rules or ranking guarantees.

## When to trigger this skill
When a target query has a featured snippet, People Also Ask, rich result, video, table, or another observable search feature that the page could legitimately support.

## Step-by-step workflow
1. Identify the active SERP feature and its current format.
2. Determine the information structure users receive: paragraph, list, table, video, definition, calculator-like result, or another format.
3. Create the clearest answer structure that satisfies the query; do not force arbitrary answer length.
4. Verify eligibility and structured-data requirements where applicable.
5. Measure the outcome and document that feature appearance is not guaranteed.

## Evidence policy

Every non-trivial SEO claim in this skill must be tagged with one of these tiers:
- **Tier 1 — Officially documented** — Google Search Central, Search Essentials, or an official Google announcement.
- **Tier 2 — Strong empirical evidence** — large-scale experiments or independent, reproducible studies.
- **Tier 3 — Industry observation** — Ahrefs, Semrush, independent SEO research, or case studies.
- **Tier 4 — Hypothesis** — plausible interpretation without strong causal proof.

When a claim cannot be cleanly supported, default to the weaker tier. At decision points, output `Evidence status: Official / Empirical / Observational / Hypothesis` and do not upgrade an inference into a fact.

**Global hard rule:** Never invent first-person experience, credentials, test results, customer outcomes, source content, or business facts. If first-hand evidence is unavailable, do not manufacture first-person experience or fabricated expertise.

## Hard rules

1. Do not present undocumented Google internal mechanisms as established facts. NavBoost, BERT, MUM, DeepRank, “pogo-sticking penalties,” leaked internal fields, or similar mechanisms may only be mentioned as **Tier 4 — Hypothesis** unless an official source documents the specific claim. **[Tier 1–4 evidence-governance rule]**
2. Never use fixed keyword-density, title-length, meta-description-length, featured-snippet-answer-length, internal-link-ratio, or article-word-count requirements as ranking rules. Use qualitative objectives: clarity, relevance, completeness for the query, reader value, natural information structure, and efficient communication. **[Tier 1 for Google not prescribing these fixed rules; Tier 4 for this governance implementation]**
3. Treat structured data as a representation layer. Implement it only when the page genuinely qualifies and the markup accurately reflects visible content. Do not claim schema independently raises rankings or AI citation likelihood. **[Tier 1]**
4. Do not promise AI Overview, AI Mode, or other generative-search visibility. Foundational SEO remains the basis: crawlability, useful content, clear answers, original evidence, coherent entities, authority, and good user experience. Any additional tactic is a hypothesis unless supported by evidence. **[Tier 1–3]**
5. Do not optimize for an AI-detector score. Optimize for evidence of real thinking, expertise, usefulness, originality, and honest limitations. **[Tier 4 internal editorial rule]**
6. Do not confuse correlation with causation. Record the observed signal separately from the interpretation and recommendation. **[Tier 2–4 evidence-governance rule]**
7. When a requested analysis depends on data the agent cannot access, label the limitation and do not fabricate the missing dataset. **[Tier 4 internal integrity rule]**
8. Before finalizing a substantive recommendation, consult `10_GOVERNANCE/evidence-engine` and, for strategy/content plans, `10_GOVERNANCE/red-team`. **[Tier 4 internal governance rule]**

## Required output format
Return: target feature; observed format; current page gap; revised structure; eligibility notes; validation plan; recommendation blocks.

### Required recommendation block

For every recommendation, output this exact structure with a blank line after it:

```text
Recommendation: <what to do>
Evidence: <what supports it>
Confidence: <percentage or High/Medium/Low>
Expected impact: <Low/Medium/High>
Risk: <Low/Medium/High>
Effort: <Low/Medium/High>
Priority: <P1/P2/P3>
Evidence status: <Official/Empirical/Observational/Hypothesis>

```

If evidence is insufficient, say so and lower confidence; do not fill the block with invented evidence.

## Evidence tier reminders
Use Tier 1 for documented Google requirements/capabilities; Tier 2 for reproducible empirical effects; Tier 3 for repeated industry observations; Tier 4 for hypotheses/internal frameworks. When uncertain, use the weaker tier. Never state a recommendation as stronger than its evidence.

## Core references

- Google Search Central — SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Google Search Central — Search Essentials: https://developers.google.com/search/docs/essentials
- Google Search Central — Spam Policies: https://developers.google.com/search/docs/essentials/spam-policies
- Google Search Central — AI Features and Your Website: https://developers.google.com/search/docs/appearance/ai-features
- Google Search Central — Canonicalization: https://developers.google.com/search/docs/crawling-indexing/canonicalization
