# Snippet Format Analysis

**Scope.** This `serp-analysis` reference is an observation tool: determine **what answer shape the current search result is using**, how stable that shape appears, and what the observation implies for the research brief. It is deliberately upstream of `serp-feature-optimization`, which handles how a target page can implement a suitable answer structure. [Evidence Tier: Tier 3 — Industry observation]

## Observation protocol

Start with the exact query and record the market, language, device, search date, and visible result types. Capture the featured answer or other prominent extraction exactly enough to identify its format: prose definition, unordered list, ordered process, table, calculator, video, or another surface. Then inspect several comparable organic results to see whether the same information shape recurs. A format observed once is evidence of the current SERP, not proof of a permanent rule. [Evidence Tier: Tier 3 — Industry observation]

Separate **format** from **content**. A list may appear because the query asks for alternatives; a table may appear because the user needs side-by-side comparison; a paragraph may be sufficient for a definition. Ask what user task the format is serving. This prevents the analyst from copying presentation without understanding why it is useful. [Evidence Tier: Tier 3 — Industry observation]

## Interpretation record

For each query, record: **observed format**, **query task**, **representative source**, **stability/variation**, **content requirement**, and **uncertainty**. If the SERP alternates between formats, report the variation. If an answer changes by location or language, preserve that distinction. Do not convert a vendor study or an SEO anecdote into a universal Google requirement. [Evidence Tier: Tier 3 — Industry observation]

## Concrete case

For “how to reset a business router,” the live SERP may show a short procedural list while the organic results contain troubleshooting guides. The analysis should tell the content strategist that the immediate task is procedural and that the page should expose an ordered method prominently. It should also note any device-specific variation visible in the results. The observation does not establish that a particular list shape causes ranking improvement. [Evidence Tier: Tier 3 — Industry observation]

## Handoff boundary

Send the observed format and task to `serp-feature-optimization` only after the SERP evidence is recorded. That downstream file decides how the target page should express the answer and whether structured data or another representation is appropriate under current documentation. [Evidence Tier: Tier 1 — Officially documented]

## Failure signatures

Common mistakes are sampling the wrong market, confusing a SERP feature with an organic-page format, copying competitor wording, and treating a temporary observation as a stable ranking law. When evidence is thin, keep the conclusion descriptive and label causal explanations as **Tier 4 — Hypothesis**. [Evidence Tier: Tier 4 — Hypothesis]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
