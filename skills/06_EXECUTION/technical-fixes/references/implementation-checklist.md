# Implementation Checklist

**Purpose.** This reference is the operating memory for `technical-fixes` when the exact job is to **translate a diagnosed technical issue into an implementation-ready change**. Use it to decide what evidence to gather, how to act on the named artifact, and what would invalidate the conclusion. It is not a claim about an undisclosed ranking formula and it does not guarantee an outcome. [Evidence Tier: Tier 3 — Industry observation]

## Use conditions

The unit of work is **implementation checklist**, not “SEO” in general. Before opening a checklist, name the URL, dataset, query group, experiment, stakeholder decision, or outreach asset under review. Record the state that exists now and the state the business or user actually needs. The distinction matters: a technically clean implementation can still be the wrong action if it serves the wrong audience, market, or commercial objective. [Evidence Tier: Tier 3 — Industry observation]

## Investigation route

- identify impacted templates and URL classes [Evidence Tier: Tier 3 — Industry observation]
- specify exact code/content/configuration change [Evidence Tier: Tier 3 — Industry observation]
- define acceptance checks and rollback [Evidence Tier: Tier 3 — Industry observation]
- assign technical owner [Evidence Tier: Tier 3 — Industry observation]

Use the action list as a sequence of observations rather than a quota. Preserve source URLs, screenshots, exports, request/response evidence, query groups, or stakeholder records that another practitioner could inspect. When first-hand evidence is unavailable, do not manufacture first-person experience, customer results, credentials, measurements, or testimonials. [Evidence Tier: Tier 1 — Officially documented]

## Specific example

For a sitemap bug, the ticket identifies the generator, the canonical URL query, exclusion rules, expected output, and post-deploy verification rather than merely saying 'fix sitemap quality'. The example is hypothetical unless the operator attaches an identifiable real source. Treat it as a pattern for reasoning, not evidence that the tactic caused a particular result. [Evidence Tier: Tier 3 — Industry observation]

## Invalid patterns

['tickets without acceptance criteria', 'changing multiple systems without sequencing', 'omitting rollback'] [Evidence Tier: Tier 3 — Industry observation]

A second class of error is methodological: confusing an observed sequence with a causal result, using a vendor benchmark as though it were universal, or converting an industry observation into a documented Google requirement. When that happens, downgrade the statement to the weaker evidence tier or remove it. [Evidence Tier: Tier 4 — Hypothesis]

## Audit note

Before handing the result to the parent skill, attach the source or measurement that supports each material conclusion and state the next validation step. Keep the recommendation separate from the evidence that motivates it. If the recommended action involves search policy, structured data, redirects, links, or generative-search visibility, verify the current official guidance before implementation. Do not imply that a structured-data field, content pattern, or outreach tactic guarantees rankings, citations, traffic, or revenue. [Evidence Tier: Tier 1 — Officially documented]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
