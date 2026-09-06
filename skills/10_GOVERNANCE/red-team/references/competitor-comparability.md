# Competitor Comparability


**Purpose.** This reference gives the `red team` skill a concrete operating method for **competitor comparability**. Use it as an internal diagnostic and decision framework; it does not represent a hidden Google ranking formula. [Evidence Tier: Tier 4 — Hypothesis]


## Adversarial competitor test

The red-team use of competitor comparability is not to build a better list of competitors; it is to **try to break the recommendation** before the recommendation is trusted. Start by hiding the competitor brand names and asking whether the selected pages still look like valid substitutes for the same user task. Then vary one dimension at a time—query intent, geography, audience sophistication, page role, monetization model, and product scope—and see whether the recommendation survives. [Evidence Tier: Tier 3 — Industry observation]

### Challenge sequence

1. **Selection bias:** Were pages chosen because they ranked well, or because they are genuinely comparable? If selection began with “top results,” add at least one challenger from the same intent class that ranks differently or has a different business model. [Evidence Tier: Tier 3 — Industry observation]
2. **Task mismatch:** Does the benchmark solve the same user problem? A product landing page and an editorial comparison may target the same noun but different decision stages. Treat them as different evidence classes. [Evidence Tier: Tier 3 — Industry observation]
3. **Authority confounding:** Could the observed advantage plausibly arise from brand, links, reputation, or product demand rather than the content change under consideration? If so, do not label the content pattern causal. [Evidence Tier: Tier 2 — Strong empirical evidence]
4. **Market confounding:** Are legal, commercial, language, pricing, or availability differences responsible for the competitor’s structure? A locally correct competitor may be unusable as a global template. [Evidence Tier: Tier 1 — Officially documented]

### Worked scenario

An SEO plan says, “Competitor A ranks first because its article contains a pricing table, so we should add the same table.” The red-team response is to inspect whether several comparable pages also use pricing tables, whether users can verify the figures, and whether the target site's products actually have stable public pricing. If the top result is a vendor with changing package pages while the target is a review site, the table may reflect business-model differences rather than a ranking requirement. The safe conclusion is narrower: **a clearly maintained pricing comparison may satisfy a visible user need**, while the causal ranking claim remains unsupported. [Evidence Tier: Tier 3 — Industry observation]

### Red flags

- A single competitor is used to justify a site-wide change. [Evidence Tier: Tier 2 — Strong empirical evidence]

The red-team closes only when alternative explanations have been considered and the surviving recommendation is phrased in proportion to the evidence. [Evidence Tier: Tier 1 — Officially documented]

## Operator notes
Select competitors by page-level comparability: query intent, audience, market, page role, and business model. Separate “content comparator” from “authority comparator” when a domain plays multiple roles. Preserve the evidence for why each benchmark belongs in the set and identify at least one plausible alternative explanation for any observed advantage. [Evidence Tier: Tier 3 — Industry observation]

## Applied scenario
For a B2B payroll query, a vendor product page, an independent review, and a government guide all appear in the SERP. The analysis treats the review as the closest content comparator, the vendor as a product comparator, and the government guide as a factual source—not three interchangeable templates. [Evidence Tier: Tier 3 — Industry observation]

## Stop conditions
Selecting only famous domains; assuming rank order proves causation; copying every visible feature; ignoring local market differences; or using one competitor to justify a sitewide rule. [Evidence Tier: Tier 3 — Industry observation]
