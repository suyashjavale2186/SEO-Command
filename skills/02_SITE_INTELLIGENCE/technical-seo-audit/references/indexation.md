# Indexation in a Technical Audit

This reference gives the technical auditor a **site-level indexation diagnosis**. It focuses on whether important URLs are eligible for indexing and whether the site's signals make the intended canonical content clear. [Evidence Tier: Tier 1 — Officially documented]

## Audit sequence
Inventory important URL classes, then inspect indexability controls such as `noindex`, canonical tags, redirects, status codes, robots rules, and sitemap inclusion. Compare intended indexation with observed Search Console states where available. [Evidence Tier: Tier 1 — Officially documented]

Pay special attention to accidental exclusion: important templates with a broad `noindex`, canonical tags pointing to unrelated URLs, redirected sitemap entries, faceted URLs creating unnecessary variants, and soft-404-like pages that look technically successful but provide little standalone value. [Evidence Tier: Tier 1 — Officially documented]

Do not treat sitemap inclusion as proof that Google indexed a URL. Sitemaps are a discovery signal; the canonical and indexation decisions are determined separately by Google's systems. [Evidence Tier: Tier 1 — Officially documented]

## Concrete scenario
An e-commerce site submits `/products/widget-blue` in the sitemap, but its canonical points to `/products/widget` while a template also emits `noindex` on filtered variants. The audit traces the signal chain and determines whether the intended canonical should be the blue variant or the parent product before proposing code changes. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes
Equating “in sitemap” with “indexed,” deleting URLs before checking demand, using robots.txt as a substitute for noindex, and relying on a single URL Inspection result as proof of sitewide behavior. [Evidence Tier: Tier 1 — Officially documented]

## Evidence boundary
Indexation behavior is documented through Search Central and first-party observations where available. Any claim about a hidden cause beyond the observable signals is a **Tier 4 — Hypothesis**. [Evidence Tier: Tier 1 — Officially documented]
