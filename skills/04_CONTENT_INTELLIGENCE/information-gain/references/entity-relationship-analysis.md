# Entity Relationship Analysis for Information Gain

**Scope.** This reference belongs to `information-gain` and answers one question: **which entities, attributes, and relationships are missing from the target content compared with the information a reader needs?** It is a content-gap method, not a database schema and not a claim about a hidden Google semantic score. [Evidence Tier: Tier 3 — Industry observation]

## Analysis model

Build a subject–predicate–object map for the topic. Add attributes to the entities and, where useful, evidence for the relationship. For an espresso machine, “machine → uses → thermoblock” is only a starting relationship; a better content model asks what the thermoblock changes, what trade-off it creates, which machine types use it, and what source supports the explanation. The goal is connected meaning, not a list of nouns. [Evidence Tier: Tier 3 — Industry observation]

Compare that map with competing pages and the actual task. Flag three kinds of omission: **missing entity**, **missing attribute**, and **missing relationship**. Then rank the gaps by reader consequence and evidence availability. A rare entity with no useful role can remain absent; a common entity that controls a purchase decision may deserve deeper treatment. [Evidence Tier: Tier 3 — Industry observation]

## Worked case

For a page about passwordless authentication, the entity map might include passkeys, authenticators, recovery methods, device enrollment, identity providers, phishing resistance, and account recovery. The useful gap may not be another definition of passkeys; it may be the relationship between recovery design and the security properties the page claims to provide. A source-backed explanation of that relationship is a stronger content contribution. [Evidence Tier: Tier 3 — Industry observation]

## Failure modes

Do not equate entity count with quality. Do not treat a private semantic framework as a documented Google scoring system. Do not add relationships merely because they are technically possible if they do not help the reader complete the task. Reject relationships that cannot be supported or that collapse meaningful distinctions into vague “related to” language. [Evidence Tier: Tier 4 — Hypothesis]

## Handoff

Return a table with **entity**, **relationship**, **reader purpose**, **evidence source**, **proposed section**, and **confidence**. That makes the output usable by the content writer and keeps the analysis auditable. [Evidence Tier: Tier 3 — Industry observation]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
