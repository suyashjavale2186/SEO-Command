# Redirect Decision for Content Updates

This reference answers **whether a content update should terminate the old URL or preserve it through a redirect**. It sits downstream of diagnosis, so its unit is a content lifecycle decision rather than technical redirect mechanics. [Evidence Tier: Tier 3 — Industry observation]

## Decision tree
Choose **refresh** when the URL still owns a useful task and needs updated substance. Choose **rewrite** when the page's core treatment is wrong but the URL still fits the topic. Choose **consolidate** when two pages genuinely overlap and one can become the clear successor. Choose **redirect** when the old URL no longer deserves to exist independently and a relevant successor can satisfy the original user need. Choose **delete** only when there is no useful successor and other business/search considerations have been checked. [Evidence Tier: Tier 3 — Industry observation]

## Concrete example
A product guide at `/guides/old-crm-migration` has no current scope after the product is retired, but `/guides/crm-migration` covers the same broader migration task. The update plan maps the retired guide to the relevant successor rather than the site's homepage. [Evidence Tier: Tier 3 — Industry observation]

## Evidence to preserve
Before redirecting, check historical organic queries, links, conversions, internal references, and whether the target actually satisfies the old page's task. Record the decision rationale so another editor can distinguish deliberate consolidation from accidental deletion. [Evidence Tier: Tier 2 — Strong empirical evidence]

## Failure modes
Redirecting every obsolete page to the homepage, combining unrelated intents, redirecting before the successor exists, and treating the absence of a 200 response as the only criterion. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
The decision framework does not expose a private Google redirect signal. Undocumented causal claims remain **Tier 4 — Hypothesis**. [Evidence Tier: Tier 1 — Officially documented]
