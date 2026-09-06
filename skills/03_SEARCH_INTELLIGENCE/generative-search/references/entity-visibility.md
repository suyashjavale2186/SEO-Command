# Entity Visibility

This reference is about **strengthening the clarity and consistency of an entity in content that may be encountered by generative-search systems**. It is an optimization/implementation reference; the measurement of whether the association appears in generated answers belongs to `generative-search-visibility/entity-association`. [Evidence Tier: Tier 3 — Industry observation]

## Entity-strengthening method
Identify the entity precisely: official name, product/service category, people, locations, parent organization, aliases, and attributes that distinguish it from similarly named entities. Use consistent factual descriptions across important first-party pages and legitimate external references. [Evidence Tier: Tier 1 — Officially documented]

Then connect the entity to the topics it genuinely serves. Explain relationships explicitly in useful prose: who the product is for, what it does, where it operates, what evidence supports its claims, and which experts or organizations are associated with it. Avoid stuffing entity names into copy merely for “semantic coverage.” [Evidence Tier: Tier 3 — Industry observation]

Structured data can represent eligible content and entities, but it is not a standalone ranking or citation guarantee. Use it only when the page qualifies and the markup matches visible content. [Evidence Tier: Tier 1 — Officially documented]

## Concrete scenario
A SaaS company is commonly referred to by both its brand and a former product name. Important pages clarify the current relationship, use the official brand consistently, identify the product category, and link to authoritative company information. The goal is factual clarity, not a promise of AI citations. [Evidence Tier: Tier 3 — Industry observation]

## Failure modes
Inconsistent names, unsupported third-party descriptions, schema that does not match visible content, invented entity relationships, and claims that entity markup “forces” AI citation. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
Generative-search behavior is partly observable but not fully specified publicly. Any claim about an internal retrieval or ranking mechanism is **Tier 4 — Hypothesis** unless officially documented. [Evidence Tier: Tier 1 — Officially documented]

## Implementation checklist
Create a single canonical description of the entity, verify names and relationships against authoritative first-party sources, and use those facts consistently where they are genuinely relevant. Strengthen the surrounding topical evidence rather than repeating the entity name without semantic purpose. [Evidence Tier: Tier 1 — Officially documented]

The implementation target is **clear association**, not forced citation. A page can explain that a product serves a particular market, show who built it, document its capabilities, and cite supporting material without claiming that those choices guarantee inclusion in a generated answer. [Evidence Tier: Tier 3 — Industry observation]
