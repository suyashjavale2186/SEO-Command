---
name: link-opportunities
description: Identify legitimate opportunities for relevant references and links while explicitly filtering out manipulative, low-value, or policy-risk tactics.
---

# Link Opportunities

## Purpose
Identify legitimate opportunities for relevant references and links while explicitly filtering out manipulative, low-value, or policy-risk tactics.

## When to trigger this skill
When planning authority acquisition or evaluating competitor link gaps.

## Step-by-step workflow
1. Inspect existing link profile evidence if available and identify meaningful topical gaps.
2. Generate opportunity classes: earned editorial mentions, relevant resource inclusion, partnerships, expert contributions, link reclamation, useful citations, and comparable tactics.
3. Evaluate each opportunity for editorial legitimacy, audience value, topical fit, likely effort, and spam-policy risk.
4. Do not promise link acquisition rates, authority-metric gains, or predictable ranking effects.
5. Prefer opportunities that would still be valuable even if no SEO benefit occurred.

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
Return: opportunity list; legitimacy assessment; outreach route; policy risk; evidence; recommendation blocks.

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

## Skill-specific hard rules
Tactics are ideas to evaluate, not guarantees. Links created primarily to manipulate rankings can violate Google spam policies.

## Core references

- Google Search Central — SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Google Search Central — Search Essentials: https://developers.google.com/search/docs/essentials
- Google Search Central — Spam Policies: https://developers.google.com/search/docs/essentials/spam-policies
- Google Search Central — AI Features and Your Website: https://developers.google.com/search/docs/appearance/ai-features
- Google Search Central — Canonicalization: https://developers.google.com/search/docs/crawling-indexing/canonicalization
