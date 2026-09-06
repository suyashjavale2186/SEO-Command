# Entity Association Measurement

This reference measures **whether a brand, product, person, or organization is actually associated with the intended topic in observed generative-search outputs**. It is a measurement task, not a prescription for how to optimize the entity. [Evidence Tier: Tier 1 — Officially documented]

## Measurement record
Create a query set that expresses the entity's important topics and customer questions. For each observed response, record the query, date, search surface, model/interface where known, whether the entity was mentioned, whether a specific page was cited, the surrounding claim, and notable competing entities. [Evidence Tier: Tier 1 — Officially documented]

Keep **mention**, **citation**, and **source-role** separate. A model may mention a business without citing its page; a cited page may support a factual statement without implying brand preference. Repeated observations are more useful than a single output because generative answers can vary. [Evidence Tier: Tier 3 — Industry observation]

## Concrete scenario
A travel platform monitors queries about rail travel in a region. Some answers mention the platform but cite government timetables and operator pages instead. The measurement log records that distinction and identifies the evidence context in which the platform is or is not selected. [Evidence Tier: Tier 3 — Industry observation]

## Failure modes
Treating one response as a trend, combining several interfaces into one score without provenance, interpreting every mention as a citation win, and inferring a hidden retrieval mechanism from a handful of examples. [Evidence Tier: Tier 3 — Industry observation]

## Evidence boundary
Google states that foundational SEO practices apply to AI features; it does not publish a simple deterministic formula for entity association. Do not claim guaranteed inclusion or a secret optimization trick. [Evidence Tier: Tier 1 — Officially documented]

## Longitudinal measurement
Store snapshots of observed answers so a later analyst can compare association changes without relying on memory. Track whether the brand is absent, mentioned, linked, or explicitly cited and preserve the surrounding claim for context. Do not collapse those states into one score unless the scoring model documents the distinction. [Evidence Tier: Tier 3 — Industry observation]

When an association disappears, inspect changes in the cited-source set, query wording, interface, and page availability before attributing the change to an optimization failure. Generative outputs are an observed surface with meaningful variability. [Evidence Tier: Tier 3 — Industry observation]
