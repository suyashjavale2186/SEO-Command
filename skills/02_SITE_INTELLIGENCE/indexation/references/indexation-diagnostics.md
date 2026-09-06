# Indexation Diagnostics

This reference is a **focused troubleshooting procedure** for a URL or URL class that is not indexed as expected. It is narrower than the technical audit: start from the observed state and trace the blocking or canonical signals one by one. [Evidence Tier: Tier 1 — Officially documented]

## Troubleshooting path
Confirm the URL returns the intended status, is crawlable, is not explicitly `noindex`, and has a sensible canonical. Check whether another URL better represents the same content and whether internal links and sitemaps reinforce the intended destination. Use Search Console evidence when available. [Evidence Tier: Tier 1 — Officially documented]

If the page is technically eligible, inspect content usefulness, duplication, and whether it is actually the intended canonical resource. Do not invent a “quality threshold” or assume that failure to index proves a hidden penalty. [Evidence Tier: Tier 1 — Officially documented]

## Concrete scenario
A help article remains absent from indexed results even though users link to it internally. Inspection finds a stale canonical pointing to an older URL. After correcting the canonical and validating the destination, the team records the change and waits for recrawling rather than adding duplicate copies of the article. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes
Making multiple SEO changes at once, submitting repeated requests without fixing the signal conflict, blocking the page in robots.txt while expecting indexing, or treating one non-indexed example as proof of a sitewide rule. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
The diagnostic can identify observable technical conflicts; it cannot expose undocumented ranking mechanisms. Such claims remain **Tier 4 — Hypothesis**. [Evidence Tier: Tier 1 — Officially documented]

## Diagnostic record
Capture the exact URL Inspection or indexation evidence, the status code, robots state, canonical target, sitemap presence, internal-link context, and any alternative URL that could be selected as the representative page. This record turns “not indexed” into a traceable technical case. [Evidence Tier: Tier 1 — Officially documented]

When several signals disagree, resolve the conflict at the source rather than adding another signal. A canonical tag pointing one way, a sitemap another way, and internal links a third way create ambiguity that should be simplified before the team assumes a content-quality problem. [Evidence Tier: Tier 3 — Industry observation]
