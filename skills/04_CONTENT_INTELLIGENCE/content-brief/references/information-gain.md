# Information Gain


**Source basis:** Ported and filtered from: skills/expert-interview/references/information-gain-writing.md, skills/semantic-gap-analysis/references/gap-classification-rubric.md. The legacy structure is retained where it is operationally useful; unsupported Google-mechanism claims and arbitrary SEO targets are not carried forward. [Evidence Tier: Tier 3 — Industry observation]


- # Technique 01: Information Gain Writing [Evidence Tier: Tier 3 — Industry observation]


- ## What It Is [Evidence Tier: Tier 3 — Industry observation]


- Writing content that adds genuinely NEW information compared to what already ranks for a keyword. Based on Google's Information Gain patent (granted June 2024), which scores how much additional value a page provides beyond existing search results. [Evidence Tier: Tier 3 — Industry observation]


- ## Why It Works [Evidence Tier: Tier 3 — Industry observation]


- The legacy source used Google's Information Gain patent as inspiration for an editorial model: compare a page with existing result coverage and look for genuinely new information. The patent does not establish a public ranking score or a guaranteed ranking effect. [Evidence Tier: Tier 4 — Hypothesis]


- The API leak confirmed this via `OriginalContentScore` — a separate metric that evaluates content uniqueness across the index. [Evidence Tier: Tier 3 — Industry observation]

## Operating context

This reference supports the `content-brief` skill when it handles **information gain**. Use the named artifact or decision as the unit of analysis and preserve provenance before acting. [Evidence Tier: Tier 3 — Industry observation]

## Field procedure
Map the subject into facts, entities, relationships, examples, decisions, exceptions, and original observations. Compare that map with the strongest competing pages, then identify what the target can substantiate that those pages do not. An information gap is valuable only when it improves the reader’s understanding or decision; a longer list of entities is not inherently better. [Evidence Tier: Tier 3 — Industry observation]

## Concrete case
A cybersecurity article explains MFA but omits recovery risks and phishing-resistant methods. The information-gap analysis adds those relationships, sources them, and uses an internal incident lesson to show why the distinction matters. [Evidence Tier: Tier 3 — Industry observation]

## Failure modes
Adding related terms with no explanatory connection; treating entity coverage as a hidden ranking threshold; copying competitor subtopics without new evidence; or inventing examples to fill a perceived gap. [Evidence Tier: Tier 3 — Industry observation]

## Topic-specific operating notes
Treat **information gain** as the concrete object of analysis within **content-brief**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant briefing from SERP evidence, user task, information gain, evidence requirements, and business role signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `content-brief/information-gain` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **information gain**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **information gain**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
