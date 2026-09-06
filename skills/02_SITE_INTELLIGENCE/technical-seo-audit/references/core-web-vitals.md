# Core Web Vitals


**Purpose.** This reference gives the `technical-seo-audit` skill a concrete operating method for **Core Web Vitals**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Evaluate user-facing loading, responsiveness, and visual stability using the current Core Web Vitals metrics and page experience evidence. [Evidence Tier: Tier 1 — Officially documented]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `core-web-vitals` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Control points
Start with field evidence where available, then isolate the page template and likely technical cause. Map the observed symptom to assets, server response, rendering work, and input handling rather than treating a single score as a diagnosis. After a change, validate the actual production template and monitor the relevant user-facing signal again. [Evidence Tier: Tier 1 — Officially documented]

## Production example
A product page has slow LCP on mobile sessions. Inspection finds a hero image several times larger than the displayed dimensions and a third-party script that blocks early rendering. The remediation prioritizes the high-cost resource and delays nonessential work, then checks production behavior after release. [Evidence Tier: Tier 2 — Strong empirical evidence]

## Failure signatures
Optimizing a lab score while field users remain slow; compressing everything without identifying the bottleneck; treating every page as the same template; or promising a ranking gain from a performance change without causal evidence. [Evidence Tier: Tier 3 — Industry observation]

## Topic-specific operating notes
Treat **core web vitals** as the concrete object of analysis within **technical-seo-audit**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant crawlability, renderability, indexability, architecture, performance, internationalization, and migrations signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `technical-seo-audit/core-web-vitals` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **core web vitals**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **core web vitals**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
