# Canonicalization


**Purpose.** This reference gives the `technical-seo-audit` skill a concrete operating method for **canonicalization**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Treat canonicalization as a duplicate-resolution system in which canonical links and redirects express preferences but Google may choose differently. [Evidence Tier: Tier 1 — Officially documented]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `canonicalization` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Analyst worksheet
For URL variants, compare the requested URL, final response URL, declared canonical, redirects, internal links, sitemap entries, and substantive content. Prefer one coherent preferred URL for materially duplicate variants and remove conflicting signals where feasible. Canonicalization should be solved together with URL generation; tagging thousands of parameter variants does not fix the system that keeps creating them. [Evidence Tier: Tier 1 — Officially documented]

## Realistic scenario
A retailer exposes a product at `/camera`, `/camera?color=black`, and `/camera?utm_source=mail`. The preferred product URL is the clean path, while campaign parameters remain tracking variants. The implementation aligns internal links and sitemap entries with the preferred URL and checks that the page renders the same intended product information. [Evidence Tier: Tier 1 — Officially documented]

## Reasons to reject the inference
Pointing a canonical at a page with materially different content; using canonicals to hide broken navigation; leaving internal links pointed at noisy variants; or treating a canonical hint as an absolute indexing command. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **canonicalization** as the concrete object of analysis within **technical-seo-audit**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant crawlability, renderability, indexability, architecture, performance, internationalization, and migrations signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `technical-seo-audit/canonicalization` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **canonicalization**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **canonicalization**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
