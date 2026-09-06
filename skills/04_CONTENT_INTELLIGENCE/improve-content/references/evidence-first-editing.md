# Evidence-First Editing




- # Technique 15: Writing Pipeline Architecture [Evidence Tier: Tier 3 — Industry observation]


- ## What It Is [Evidence Tier: Tier 3 — Industry observation]


- A multi-phase, multi-agent pipeline for producing high-quality SEO content. Based on analysis of 15+ agentic writing systems, this architecture represents the consensus best approach: specialized phases with quality gates, not a single monolithic generation. [Evidence Tier: Tier 3 — Industry observation]


- ## Why It Works [Evidence Tier: Tier 3 — Industry observation]


- Research consistently shows that multi-agent pipelines outperform single-prompt generation: [Evidence Tier: Tier 3 — Industry observation]


- - Section-by-section generation maintains quality over long articles [Evidence Tier: Tier 3 — Industry observation]


- - Specialized agents (writer vs. critic) produce better results than a generalist [Evidence Tier: Tier 3 — Industry observation]


- - Iterative revision can improve quality, but the useful stopping rule is evidence and defect reduction rather than a predetermined number of cycles. [Evidence Tier: Tier 2 — Strong empirical evidence]


- - Quality gates prevent bad content from being output [Evidence Tier: Tier 3 — Industry observation]

## Operating context

This reference supports the `improve-content` skill when it handles **evidence first editing**. Use the named artifact or decision as the unit of analysis and preserve provenance before acting. [Evidence Tier: Tier 3 — Industry observation]

## Analyst worksheet
For every substantive claim, trace it to a source and classify the support: Tier 1 official documentation, Tier 2 strong empirical evidence, Tier 3 industry observation, or Tier 4 hypothesis. If a source mixes observation and speculation, classify the relevant sentence at the weaker level rather than inheriting the source’s confidence. [Evidence Tier: Tier 1 — Officially documented]

## Realistic scenario
A vendor article says “our pages rank because of X.” The evidence engine may retain the vendor’s observation as Tier 3, but it must not restate an inferred private ranking mechanism as fact. If the mechanism cannot be independently supported, the recommendation should focus on the observable practice rather than the claimed internal signal. [Evidence Tier: Tier 1 — Officially documented]

## Reasons to reject the inference
Upgrading evidence because a claim is repeated across many sites; treating a tool score as official Google data; hiding uncertainty in footnotes; or allowing a hypothesis to become a fact through copied templates. [Evidence Tier: Tier 1 — Officially documented]

## Topic-specific operating notes
Treat **evidence first editing** as the concrete object of analysis within **improve-content**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant performance-led updates, content decay, evidence gaps, freshness, and preservation of successful intent coverage signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `improve-content/evidence-first-editing` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **evidence first editing**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **evidence first editing**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
