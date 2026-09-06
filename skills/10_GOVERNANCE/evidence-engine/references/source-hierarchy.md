# Source Hierarchy

**Scope.** `evidence-engine/source-hierarchy` decides **which kind of source should be preferred for a particular kind of claim** before fact-checking begins. Its job is source selection and provenance design; it does not verify the truth of each sentence—that is the specialized role of `fact-checking/source-verification`. [Evidence Tier: Tier 3 — Industry observation]

## Match source to claim

Use the most authoritative source appropriate to the proposition. Official Google documentation is the preferred source for documented Search behavior and policy. A regulator or standards body is the preferred source for its own rules. A company's product documentation is strongest for its own current functionality. A CRM or finance system is strongest for a first-party business metric. A reproducible independent study is stronger for an empirical effect than a vendor marketing page. [Evidence Tier: Tier 1 — Officially documented]

Source hierarchy is conditional, not a universal ranking of websites. A vendor may be the primary source for its own product specification while being a weak source for claims about the broader market. Likewise, an SEO industry study can be useful for an observational benchmark but cannot override an official Google statement about a documented policy. [Evidence Tier: Tier 3 — Industry observation]

## Provenance record

For each material claim, store **claim type**, **preferred source class**, **actual source**, **publication/update date**, **scope**, and **evidence tier**. If the ideal source is unavailable, record the substitution. That record lets later editors understand why a Tier 3 observation was used and prevents a weak secondary article from silently becoming a Tier 1-looking citation. [Evidence Tier: Tier 3 — Industry observation]

## Concrete case

The team needs three different sources for one article: official Search Central guidance for canonicalization, the company's product documentation for its API behavior, and internal sales data for close rates. An industry blog may explain context around all three, but it should not become the authority for claims owned by those primary sources. The hierarchy therefore changes by claim, even inside one paragraph. [Evidence Tier: Tier 1 — Officially documented]

## Failure modes

Do not select a source because it ranks highly in search. Do not treat a highly linked page as automatically authoritative. Do not use a source outside its scope merely because its prose is clearer. Do not collapse source quality and claim truth into one score; a strong source can still be misquoted or outdated, which is why `source-verification` remains a separate step. [Evidence Tier: Tier 3 — Industry observation]

**Evidence status:** Official / Empirical / Observational / Hypothesis, assigned claim by claim above.
