# Javascript Rendering


**Purpose.** This reference gives the `technical-seo-audit` skill a concrete operating method for **JavaScript rendering**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Make critical content and navigation available in rendered HTML and verify what Google can actually access and render. [Evidence Tier: Tier 1 — Officially documented]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `javascript-rendering` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Field procedure
Compare server-delivered HTML with rendered DOM for navigation, canonical tags, structured data, primary content, and important links. Identify whether JavaScript merely enhances an accessible page or is necessary to expose content that should be discoverable. Verify that client-side routing returns appropriate URLs and that important content does not disappear when scripts fail or are delayed. [Evidence Tier: Tier 1 — Officially documented]

## Concrete case
A knowledge-base application renders article bodies only after a client request, while the initial HTML contains an empty shell. The audit checks rendered content and link discovery, then recommends server-visible article content and crawlable navigation rather than adding more client-side prefetching. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes
Assuming “the browser displays it” means a crawler can reliably process it; hiding canonicals or links behind interaction-only code; relying on hash fragments for primary URLs; and fixing rendering by adding more JavaScript. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **javascript rendering** as the concrete object of analysis within **technical-seo-audit**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant crawlability, renderability, indexability, architecture, performance, internationalization, and migrations signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `technical-seo-audit/javascript-rendering` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **javascript rendering**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **javascript rendering**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
