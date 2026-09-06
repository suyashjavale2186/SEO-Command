# Evidence Tiers


**Purpose.** This reference gives the `evidence engine` skill a concrete operating method for **evidence tiers**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Tier 1 is official Google documentation or announcements; Tier 2 is strong empirical evidence; Tier 3 is industry observation; Tier 4 is hypothesis. [Evidence Tier: Tier 3 — Industry observation]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

## Operating context

This reference supports the `evidence-engine` skill when it handles **evidence tiers**. Use the named artifact or decision as the unit of analysis and preserve provenance before acting. [Evidence Tier: Tier 3 — Industry observation]

## Decision procedure
For every substantive claim, trace it to a source and classify the support: Tier 1 official documentation, Tier 2 strong empirical evidence, Tier 3 industry observation, or Tier 4 hypothesis. If a source mixes observation and speculation, classify the relevant sentence at the weaker level rather than inheriting the source’s confidence. [Evidence Tier: Tier 1 — Officially documented]

## Case study
A vendor article says “our pages rank because of X.” The evidence engine may retain the vendor’s observation as Tier 3, but it must not restate an inferred private ranking mechanism as fact. If the mechanism cannot be independently supported, the recommendation should focus on the observable practice rather than the claimed internal signal. [Evidence Tier: Tier 1 — Officially documented]

## Common failure modes
Upgrading evidence because a claim is repeated across many sites; treating a tool score as official Google data; hiding uncertainty in footnotes; or allowing a hypothesis to become a fact through copied templates. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **evidence tiers** as the concrete object of analysis within **evidence-engine**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant claim classification, source quality, provenance, confidence, and recommendation evidence signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `evidence-engine/evidence-tiers` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **evidence tiers**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **evidence tiers**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
