# Redirects

Use this reference to audit whether old URLs lead users and crawlers to the **correct successor resource**. The key concern is continuity of user intent, not a target count of redirects. [Evidence Tier: Tier 1 — Officially documented]

## Audit method
Map source URL → redirect behavior → final URL. Distinguish direct redirects, chains, loops, wrong-topic destinations, and missing mappings. For migrations, keep a source-to-target table and test important legacy URLs before launch. Then update internal links, sitemaps, feeds, and references so the site points directly to the intended destination. [Evidence Tier: Tier 1 — Officially documented]

## Concrete example
A documentation migration sends `/docs/install-old` to `/docs/v2`, which then redirects to `/products/platform`. The final product page is not the true successor to the installation guide. The correct fix is a direct mapping to the new installation page, followed by validation of internal links. [Evidence Tier: Tier 1 — Officially documented]

## Decision cues
Use a redirect when a page has a clear replacement or a deliberate URL change. Do not redirect unrelated pages merely to avoid a 404, and do not use a homepage as a universal destination. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes
Redirect loops, stacked migration chains, irrelevant destinations, forgotten old URLs, and source maps that disappear before production verification are common operational risks. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
Redirect behavior is documented; its contribution to any undisclosed ranking calculation is not. Any such explanation is **Tier 4 — Hypothesis**. [Evidence Tier: Tier 1 — Officially documented]

## Audit handoff
For a redirect review, save the old URL, response chain, final status, destination relevance, and any internal links still pointing at the old address. This makes the issue actionable for engineering and distinguishes a deliberate redirect from an accidental chain. [Evidence Tier: Tier 1 — Officially documented]

During migration work, group redirects by template or business reason only after verifying that the mappings are genuinely equivalent. A rule that is safe for one legacy path can misroute another path with a different user task, so sampled validation must reflect the actual URL classes present on the site. [Evidence Tier: Tier 3 — Industry observation]
