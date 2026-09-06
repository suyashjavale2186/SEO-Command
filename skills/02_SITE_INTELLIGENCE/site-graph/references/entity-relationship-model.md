# Entity Relationship Model for the Site Graph

**Scope.** This `site-graph` reference models relationships **between site-level objects** so the graph can support navigation, ownership, query mapping, and diagnosis. Its job is architectural: represent topics, pages, queries, competitors, links, authors, and conversions as nodes and meaningful relationships as edges. It is distinct from `information-gain/entity-relationship-analysis`, which examines missing meaning inside content. [Evidence Tier: Tier 3 — Industry observation]

## Graph schema

Represent a page as connected to its primary topic, target query cluster, canonical URL, business owner, author or reviewer, related pages, conversion event, and relevant competitor set. Represent a topic as connected to parent and child topics, supporting pages, and demand evidence. Represent a query cluster as connected to pages that currently attract impressions or rankings. Store the source of each relationship so a graph edge is not mistaken for objective truth. [Evidence Tier: Tier 3 — Industry observation]

The most useful edges answer operational questions. **Page → targets → query cluster** supports search mapping. **Page → links to → page** exposes the internal-link graph. **Page → supports → conversion** connects content to business value. **Topic → contains → page** reveals weak hubs or isolated spokes. **Competitor → ranks for → query cluster** frames competitive context without assuming two domains are otherwise equivalent. [Evidence Tier: Tier 3 — Industry observation]

## Graph validation

A relationship should have a clear direction and reason. “Page A relates to Page B” is weak because it cannot explain what the relationship means. “Page A links contextually to Page B because B resolves the next decision introduced by A” is operationally useful. When a relationship is inferred rather than observed—such as a topic grouping created from semantic similarity—mark it as inferred and store the rule that created it. [Evidence Tier: Tier 4 — Hypothesis]

## Concrete case

A software site has a topic hub for “inventory management” connected to guides on stock forecasting, barcode workflows, warehouse integrations, and vendor selection. One high-value guide has no inbound contextual links and no mapped conversion path. The graph makes the problem visible as a missing edge rather than as a vague “weak content” judgment. The site-graph skill can then pass the exact relationship to the internal-link or strategy skill. [Evidence Tier: Tier 3 — Industry observation]

## Failure modes

Do not use a graph edge as proof of causality. Do not create thousands of weak semantic edges merely to make a graph look complete. Do not overwrite the canonical source with a derived label. The graph is a decision aid; its value comes from traceable relationships that support an actual diagnosis or action. [Evidence Tier: Tier 3 — Industry observation]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
