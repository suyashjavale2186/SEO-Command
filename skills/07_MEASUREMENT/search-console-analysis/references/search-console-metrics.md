# Search Console Metrics


**Purpose.** This reference gives the `search-console-analysis` skill a concrete operating method for **Search Console metrics**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Interpret clicks, impressions, CTR, and average position in context rather than as direct measures of quality. [Evidence Tier: Tier 1 — Officially documented]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `search-console-metrics` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Evidence map
Use Search Console fields according to the question being answered: queries for demand and query-page matching, pages for landing-page opportunity, impressions and clicks for visibility, CTR for snippet performance, position as a directional outcome, and search appearance for feature context. Pair performance tables with the actual URL and query group so the recommendation can be audited. [Evidence Tier: Tier 1 — Officially documented]

## Practical case
A page receives many impressions for a query but few clicks while another page on the same domain receives most clicks. The analyst checks query-page alignment and current SERP presentation before changing content, rather than interpreting impressions alone as success. [Evidence Tier: Tier 1 — Officially documented]

## Disqualifiers
Treating average position as a precise universal rank; aggregating unrelated queries; comparing periods with different indexing states; or ignoring the Search Console query/page relationship when diagnosing cannibalization. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **search console metrics** as the concrete object of analysis within **search-console-analysis**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant queries, pages, impressions, clicks, CTR, position, indexation, search appearance, and change analysis signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `search-console-analysis/search-console-metrics` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **search console metrics**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **search console metrics**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
