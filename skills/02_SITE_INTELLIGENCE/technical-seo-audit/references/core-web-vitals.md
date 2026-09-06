# Core Web Vitals

**Purpose.** This reference is the operating memory for `technical-seo-audit` when the exact job is to **diagnose actual user-facing performance bottlenecks**. Use it to decide what evidence to gather, how to act on the named artifact, and what would invalidate the conclusion. It is not a claim about an undisclosed ranking formula and it does not guarantee an outcome. [Evidence Tier: Tier 3 — Industry observation]

## What to capture

The unit of work is **core web vitals**, not “SEO” in general. Before opening a checklist, name the URL, dataset, query group, experiment, stakeholder decision, or outreach asset under review. Record the state that exists now and the state the business or user actually needs. The distinction matters: a technically clean implementation can still be the wrong action if it serves the wrong audience, market, or commercial objective. [Evidence Tier: Tier 3 — Industry observation]

## Field method

- separate field data from lab diagnostics [Evidence Tier: Tier 3 — Industry observation]
- trace LCP, INP, and CLS symptoms to the page template and resource causing them [Evidence Tier: Tier 3 — Industry observation]
- validate the production change rather than assuming a score change proves business impact [Evidence Tier: Tier 3 — Industry observation]

Use the action list as a sequence of observations rather than a quota. Preserve source URLs, screenshots, exports, request/response evidence, query groups, or stakeholder records that another practitioner could inspect. When first-hand evidence is unavailable, do not manufacture first-person experience, customer results, credentials, measurements, or testimonials. [Evidence Tier: Tier 1 — Officially documented]

## Worked case

A commerce template shows slow LCP because the hero image is fetched late and a consent bundle blocks main-thread work; the useful action is to trace those dependencies and validate the shipped template, not to rewrite copy because the page 'feels slow'. The example is hypothetical unless the operator attaches an identifiable real source. Treat it as a pattern for reasoning, not evidence that the tactic caused a particular result. [Evidence Tier: Tier 3 — Industry observation]

## Do-not-do list

['optimizing a lab score with no user evidence', 'treating a single metric as a complete diagnosis', 'claiming a ranking gain without causal evidence'] [Evidence Tier: Tier 3 — Industry observation]

A second class of error is methodological: confusing an observed sequence with a causal result, using a vendor benchmark as though it were universal, or converting an industry observation into a documented Google requirement. When that happens, downgrade the statement to the weaker evidence tier or remove it. [Evidence Tier: Tier 4 — Hypothesis]

## Review notes

Before handing the result to the parent skill, attach the source or measurement that supports each material conclusion and state the next validation step. Keep the recommendation separate from the evidence that motivates it. If the recommended action involves search policy, structured data, redirects, links, or generative-search visibility, verify the current official guidance before implementation. Do not imply that a structured-data field, content pattern, or outreach tactic guarantees rankings, citations, traffic, or revenue. [Evidence Tier: Tier 1 — Officially documented]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
