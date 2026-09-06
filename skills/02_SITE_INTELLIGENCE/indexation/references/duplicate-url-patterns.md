# Duplicate Url Patterns


**Purpose.** This reference gives the `indexation` skill a concrete operating method for **duplicate URL patterns**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Catalog duplicates created by parameters, filters, protocol/host variants, localization, alternate paths, and accidental duplicates. [Evidence Tier: Tier 3 — Industry observation]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `duplicate-url-patterns` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Implementation guide
Work from URL-level evidence: crawlability, response status, robots directives, noindex signals, canonicalization, sitemap presence, and Search Console coverage information where available. Distinguish “not indexed” from “not eligible to be indexed” and distinguish an excluded duplicate from a technical error. The remedy depends on the state, so do not recommend content changes until indexability has been established as the constraint. [Evidence Tier: Tier 1 — Officially documented]

## Specific example
A SaaS site has a new documentation page returning `200`, linked from the navigation, included in the sitemap, but Search Console reports it as excluded because another canonical URL is selected. The correct response is to reconcile the canonical and content relationship rather than simply resubmitting the URL. [Evidence Tier: Tier 1 — Officially documented]

## Red flags
Treating every excluded URL as an error; assuming sitemap submission forces indexing; changing content to solve a robots/noindex problem; or confusing a canonicalized duplicate with a missing page. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **duplicate url patterns** as the concrete object of analysis within **indexation**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant discovery, crawling, canonical selection, indexing states, sitemaps, and Search Console evidence signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `indexation/duplicate-url-patterns` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **duplicate url patterns**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **duplicate url patterns**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
