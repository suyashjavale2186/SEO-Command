# Migration Seo


**Purpose.** This reference gives the `technical-seo-audit` skill a concrete operating method for **migration SEO**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Core principles


- Preserve URL meaning, redirects, internal links, canonicals, sitemaps, and monitoring during domain, protocol, template, or path migrations. [Evidence Tier: Tier 3 — Industry observation]


- Record evidence before scoring or recommending changes. The strongest evidence is primary documentation, direct first-party data, reproducible measurement, or clearly attributed expert evidence; weaker evidence should remain labeled as such. [Evidence Tier: Tier 1 — Officially documented]


- Keep observed facts, interpretations, forecasts, and hypotheses in separate fields. This prevents a plausible explanation from becoming an unsupported fact merely through repetition. [Evidence Tier: Tier 4 — Hypothesis]


- Never invent first-person experience, customer results, credentials, testimonials, measurements, or screenshots. When first-hand evidence is unavailable, write from sourced information and say what is missing. [Evidence Tier: Tier 1 — Officially documented]

**Source basis:** New guidance for the Elite architecture; no direct legacy equivalent was available. The procedures below are deliberately specific to `migration-seo` and should be used as an operating aid, not as a claim about a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]

## Operator notes
Create a source-to-destination inventory for every important URL class. For each mapping, record old URL, intended replacement, redirect behavior, canonical expectations, internal-link changes, traffic or conversion role, and validation evidence. Sample representative templates—not just the most famous URLs—and include a rollback plan before the cutover. [Evidence Tier: Tier 1 — Officially documented]

## Applied scenario
An education platform moves `/courses/python-1` to `/learning/python-basics`. The migration map preserves the page’s intent, updates internal links, redirects the old route directly, and checks that the new page contains the core material students expected. A separate archive page is deliberately mapped elsewhere rather than forcing every old route onto one generic destination. [Evidence Tier: Tier 3 — Industry observation]

## Stop conditions
Redirecting every old URL to the homepage; losing query-bearing or localized variants; failing to update internal links; measuring the migration only from overall traffic; or declaring success before production responses and analytics are validated. [Evidence Tier: Tier 2 — Strong empirical evidence]

## Topic-specific operating notes
Treat **migration seo** as the concrete object of analysis within **technical-seo-audit**. Work from the artifact that the file names—rather than from a generic SEO checklist—and preserve the field-level evidence that another practitioner would need to reproduce the judgment. For this topic, inspect the relevant crawlability, renderability, indexability, architecture, performance, internationalization, and migrations signals first, then test the business or user consequence of the observed issue. [Evidence Tier: Tier 3 — Industry observation]

When the evidence is incomplete, name the missing field or source explicitly and state what observation would change the conclusion. Do not substitute a vendor benchmark, an internal score, or a plausible Google explanation for missing evidence. [Evidence Tier: Tier 1 — Officially documented]

### Concrete operator case
Imagine a real but hypothetical organization using `technical-seo-audit/migration-seo` as part of an SEO review. The operator records the current state, isolates the specific variable relevant to **migration seo**, compares it with the intended user/business outcome, and chooses an action that can later be validated. The example is illustrative only; it must never be presented as a real client result or invented first-hand experience. [Evidence Tier: Tier 3 — Industry observation]

### Topic-specific failure modes
Watch for the characteristic mistake of **migration seo**: applying the concept to the wrong artifact, treating a proxy metric as the outcome, copying a competitor pattern without proving comparability, or turning a hypothesis into an assertion. Also stop when the proposed action would require fabricated evidence, violate search-policy guidance, or imply a guaranteed ranking or revenue result. [Evidence Tier: Tier 1 — Officially documented]
