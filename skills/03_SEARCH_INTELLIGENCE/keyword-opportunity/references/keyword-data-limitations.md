# Keyword Data Limitations


**Source basis:** Ported and filtered from: skills/keyword-deep-dive/references/difficulty-from-serp-signals.md, skills/keyword-deep-dive/references/ctr-benchmarks-by-position.md. The legacy structure is retained where it is operationally useful; unsupported Google-mechanism claims and arbitrary SEO targets are not carried forward. [Evidence Tier: Tier 3 — Industry observation]


- # Difficulty From SERP Signals [Evidence Tier: Tier 3 — Industry observation]


- How to classify a keyword as Easy, Moderate, or Hard by reading the actual SERP instead of trusting a KD score from a paid tool. [Evidence Tier: Tier 3 — Industry observation]


- ## Why We Reject KD Scores [Evidence Tier: Tier 3 — Industry observation]


- KD scores from Ahrefs, Moz, and Semrush are modeled estimates built from different formulas. Ahrefs leans primarily on referring domains; Semrush blends backlink strength with keyword characteristics. There's no industry-standard formula, and [Keywords Everywhere's comparison](https://keywordseverywhere.com/blog/how-the-top-tools-calculate-kd/) notes the tools can differ by 30+ points on the same keyword. A KD of 15 in one tool can be a KD of 55 in another. That's not a minor disagreement; it's a signal that the metric isn't measuring what you care about. [Evidence Tier: Tier 3 — Industry observation]

## Operating context

This reference supports the `keyword-opportunity` skill when it handles **keyword data limitations**. Use the named artifact or decision as the unit of analysis and preserve provenance before acting. [Evidence Tier: Tier 3 — Industry observation]

## Control points
Document what your keyword source can and cannot tell you. Volume may be modeled, aggregated, delayed, or unavailable for long-tail queries; difficulty metrics are vendor-specific and not Google ranking scores. Use external keyword metrics as directional evidence, then combine them with observed SERPs, first-party queries, business value, and feasibility. [Evidence Tier: Tier 3 — Industry observation]

## Production example
A niche compliance query has little third-party volume data but appears repeatedly in Search Console impressions and sales-call notes. The analysis does not reject it because an external tool shows “no volume”; instead it treats the first-party evidence as stronger for that site-specific opportunity. [Evidence Tier: Tier 2 — Strong empirical evidence]

## Failure signatures
Presenting vendor metrics as Google measurements; inventing volume for missing data; ranking opportunities by search volume alone; or hiding the data source and date behind a polished final score. [Evidence Tier: Tier 3 — Industry observation]

## Topic-specific operating notes
Treat **keyword data limitations** as the concrete object of analysis within **keyword-opportunity**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant demand evidence, query intent, feasibility, business value, and information advantage signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `keyword-opportunity/keyword-data-limitations` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **keyword data limitations**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **keyword data limitations**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
