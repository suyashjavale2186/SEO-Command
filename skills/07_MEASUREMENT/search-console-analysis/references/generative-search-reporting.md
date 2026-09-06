# Generative Search Reporting in Search Console

Use this reference to interpret **first-party reporting about generative-search visibility** without mixing it with ordinary organic ranking metrics. The measurement job is to preserve what the reporting surface actually exposes and avoid inventing fields it does not provide. [Evidence Tier: Tier 1 — Officially documented]

## Reporting method
Record the date range, property, page/query filters, search appearance or generative feature where exposed, and the resulting impressions/clicks or other documented fields. Keep generative-search observations separate from traditional organic observations when the platform distinguishes them. [Evidence Tier: Tier 1 — Officially documented]

Compare trends, query themes, and landing pages rather than collapsing everything into one “AI visibility” score. When the interface or documentation changes, update the measurement definition instead of silently treating the new data as comparable to an old series. [Evidence Tier: Tier 1 — Officially documented]

## Concrete example
A site sees new generative-search reporting tied to queries that already drive organic traffic. The analyst logs the generative surface separately, then checks whether the cited/visible pages overlap with the pages receiving ordinary Search traffic. The analysis describes the observed relationship without claiming the generative feature used a particular private retrieval mechanism. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes
Do not treat a reported generative impression as an organic position, infer citation quality from click count alone, or compare metrics across different definitions without documenting the change. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
Use Google's published documentation for field definitions. Any additional causal story about AI retrieval or ranking is **Tier 4 — Hypothesis** unless officially supported. [Evidence Tier: Tier 1 — Officially documented]

## Reporting change control
When Google changes a Search Console reporting surface, snapshot the old field definitions and note the migration date before extending a historical dashboard. Avoid pretending that a newly defined generative-search metric is directly comparable with an older organic metric merely because both are labeled “impressions” or “clicks.” [Evidence Tier: Tier 1 — Officially documented]

A measurement note should state exactly what the interface exposes, what it does not expose, and which interpretations remain observational. This is especially important for generative features where visible answers and citations can vary across interfaces and time. [Evidence Tier: Tier 1 — Officially documented]
