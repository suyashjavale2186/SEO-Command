# AUDIT REPORT — SuperSEO Elite v4

## Method

This audit was run against the packaged working tree immediately before ZIP creation. Reference word counts use Python `re` with `\b[\w’'-]+\b` over UTF-8 Markdown text; headings, inline code, labels, and Evidence Tier tags are included, and no file content is excluded. Similarity uses `sklearn==1.8.0`, `TfidfVectorizer(stop_words='english')`, then pairwise cosine similarity. Only pairs belonging to different skill folders are compared. With 181 reference files, this produces 15,979 cross-skill pairs. No sampling was used for the population result.

## Reference depth

- Reference files: **181**
- Total reference words: **93,950**
- Minimum: **304**
- Maximum: **786**
- Files below 300: **0**
- Files above 800: **0**


## Per-skill counts

| Skill | Ref files | Min words | Max words | Total words |
|---|---:|---:|---:|---:|

| `01_BUSINESS_INTELLIGENCE/audience-model` | 3 | 473 | 481 | 1,429 |
| `01_BUSINESS_INTELLIGENCE/business-context` | 3 | 484 | 486 | 1,455 |
| `01_BUSINESS_INTELLIGENCE/conversion-model` | 3 | 369 | 489 | 1,339 |
| `02_SITE_INTELLIGENCE/cannibalization` | 4 | 481 | 502 | 1,955 |
| `02_SITE_INTELLIGENCE/indexation` | 4 | 367 | 490 | 1,821 |
| `02_SITE_INTELLIGENCE/internal-links` | 4 | 597 | 626 | 2,452 |
| `02_SITE_INTELLIGENCE/site-graph` | 4 | 434 | 641 | 2,316 |
| `02_SITE_INTELLIGENCE/technical-seo-audit` | 8 | 352 | 504 | 3,677 |
| `03_SEARCH_INTELLIGENCE/competitor-analysis` | 4 | 304 | 775 | 2,242 |
| `03_SEARCH_INTELLIGENCE/generative-search` | 4 | 403 | 615 | 2,232 |
| `03_SEARCH_INTELLIGENCE/intent-analysis` | 4 | 322 | 623 | 2,185 |
| `03_SEARCH_INTELLIGENCE/keyword-opportunity` | 4 | 409 | 638 | 2,295 |
| `03_SEARCH_INTELLIGENCE/serp-analysis` | 5 | 351 | 616 | 2,628 |
| `03_SEARCH_INTELLIGENCE/serp-feature-optimization` | 4 | 341 | 631 | 2,080 |
| `04_CONTENT_INTELLIGENCE/content-brief` | 5 | 409 | 620 | 2,465 |
| `04_CONTENT_INTELLIGENCE/eeat` | 5 | 553 | 620 | 2,943 |
| `04_CONTENT_INTELLIGENCE/expert-interview` | 6 | 417 | 649 | 3,320 |
| `04_CONTENT_INTELLIGENCE/improve-content` | 5 | 316 | 627 | 2,549 |
| `04_CONTENT_INTELLIGENCE/information-gain` | 4 | 373 | 622 | 2,207 |
| `04_CONTENT_INTELLIGENCE/write-content` | 8 | 383 | 749 | 4,739 |
| `05_AUTHORITY/authority-analysis` | 4 | 363 | 786 | 2,342 |
| `05_AUTHORITY/digital-pr` | 4 | 486 | 501 | 1,975 |
| `05_AUTHORITY/link-opportunities` | 5 | 404 | 633 | 2,873 |
| `06_EXECUTION/content-updates` | 6 | 401 | 740 | 3,109 |
| `06_EXECUTION/internal-link-actions` | 3 | 495 | 508 | 1,503 |
| `06_EXECUTION/publishing-plan` | 3 | 338 | 697 | 1,525 |
| `06_EXECUTION/technical-fixes` | 3 | 471 | 481 | 1,431 |
| `07_MEASUREMENT/analytics-analysis` | 4 | 368 | 488 | 1,828 |
| `07_MEASUREMENT/content-decay` | 4 | 394 | 502 | 1,888 |
| `07_MEASUREMENT/conversions` | 3 | 475 | 487 | 1,442 |
| `07_MEASUREMENT/generative-search-visibility` | 4 | 373 | 491 | 1,838 |
| `07_MEASUREMENT/search-console-analysis` | 4 | 368 | 490 | 1,740 |
| `08_EXPERIMENTATION/hypothesis` | 3 | 484 | 741 | 1,711 |
| `08_EXPERIMENTATION/learning` | 3 | 474 | 484 | 1,436 |
| `08_EXPERIMENTATION/measurement` | 3 | 478 | 488 | 1,451 |
| `08_EXPERIMENTATION/seo-experiment` | 4 | 485 | 621 | 2,090 |
| `09_STRATEGY/opportunity-scoring` | 4 | 320 | 631 | 1,789 |
| `09_STRATEGY/prioritization` | 3 | 484 | 497 | 1,475 |
| `09_STRATEGY/seo-roadmap` | 4 | 333 | 696 | 1,986 |
| `10_GOVERNANCE/evidence-engine` | 5 | 401 | 624 | 2,397 |
| `10_GOVERNANCE/fact-checking` | 3 | 391 | 761 | 1,788 |
| `10_GOVERNANCE/red-team` | 4 | 485 | 618 | 2,311 |
| `10_GOVERNANCE/risk-detection` | 4 | 378 | 612 | 1,938 |
| `10_GOVERNANCE/seo-myth-detection` | 3 | 476 | 641 | 1,755 |

## Similarity audit

- Population: **15,979** cross-skill reference-file pairs
- Average cosine similarity: **0.331990**
- Maximum cosine similarity: **0.698776**
- Pairs above 0.70: **0**
- Pairs above 0.75: **0**
- Pairs above 0.80: **0**
- Complete list above 0.70: **none**


### Highest-scoring pairs (all below 0.70)

| Cosine | File A | File B |
|---:|---|---|

| 0.698776 | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` | `skills/08_EXPERIMENTATION/seo-experiment/references/experiment-record.md` |
| 0.696841 | `skills/08_EXPERIMENTATION/measurement/references/baseline-methodology.md` | `skills/07_MEASUREMENT/content-decay/references/baseline-comparison.md` |
| 0.690133 | `skills/04_CONTENT_INTELLIGENCE/content-brief/references/serp-driven-briefing.md` | `skills/04_CONTENT_INTELLIGENCE/write-content/references/serp-driven-writing.md` |
| 0.689417 | `skills/10_GOVERNANCE/evidence-engine/references/evidence-tiers.md` | `skills/04_CONTENT_INTELLIGENCE/write-content/references/evidence-first-writing.md` |
| 0.688805 | `skills/08_EXPERIMENTATION/seo-experiment/references/internal-link-tests.md` | `skills/02_SITE_INTELLIGENCE/internal-links/references/internal-link-graph.md` |
| 0.685226 | `skills/06_EXECUTION/technical-fixes/references/validation.md` | `skills/10_GOVERNANCE/evidence-engine/references/claim-verification.md` |
| 0.684892 | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` | `skills/08_EXPERIMENTATION/seo-experiment/references/content-tests.md` |
| 0.683233 | `skills/06_EXECUTION/content-updates/references/delete.md` | `skills/08_EXPERIMENTATION/seo-experiment/references/experiment-record.md` |
| 0.681626 | `skills/06_EXECUTION/technical-fixes/references/validation.md` | `skills/06_EXECUTION/content-updates/references/delete.md` |
| 0.679627 | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` | `skills/07_MEASUREMENT/generative-search-visibility/references/measurement-limitations.md` |
| 0.679262 | `skills/06_EXECUTION/content-updates/references/delete.md` | `skills/10_GOVERNANCE/evidence-engine/references/claim-verification.md` |
| 0.677523 | `skills/02_SITE_INTELLIGENCE/internal-links/references/internal-link-graph.md` | `skills/02_SITE_INTELLIGENCE/site-graph/references/graph-diagnostics.md` |
| 0.677376 | `skills/06_EXECUTION/technical-fixes/references/implementation-checklist.md` | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` |
| 0.676315 | `skills/06_EXECUTION/content-updates/references/refresh.md` | `skills/10_GOVERNANCE/evidence-engine/references/claim-verification.md` |
| 0.673730 | `skills/10_GOVERNANCE/risk-detection/references/implementation-risk.md` | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` |
| 0.672230 | `skills/06_EXECUTION/content-updates/references/consolidate.md` | `skills/08_EXPERIMENTATION/seo-experiment/references/experiment-record.md` |
| 0.670187 | `skills/06_EXECUTION/content-updates/references/delete.md` | `skills/07_MEASUREMENT/search-console-analysis/references/query-analysis.md` |
| 0.668727 | `skills/08_EXPERIMENTATION/seo-experiment/references/content-tests.md` | `skills/07_MEASUREMENT/search-console-analysis/references/query-analysis.md` |
| 0.668398 | `skills/06_EXECUTION/content-updates/references/update-decision-tree.md` | `skills/07_MEASUREMENT/generative-search-visibility/references/measurement-limitations.md` |
| 0.668247 | `skills/06_EXECUTION/content-updates/references/delete.md` | `skills/08_EXPERIMENTATION/hypothesis/references/experiment-design.md` |

## Governance / placeholder / integrity checks

- Canonical `governance-contract.md` files: **1**
- Literal `legacy-source marker`: **0**
- Literal `broken template phrase`: **0**
- Empty level-2 headings: **0**
- Reference paragraphs of substantive length without an Evidence Tier tag: **0**
- Unlabeled Google mechanism terms (NavBoost/BERT/MUM/DeepRank/pogo-sticking/OriginalContentScore): **0**
- SKILL.md files: **44**
- SKILL.md files identical to approved v2: **44 / 44**
- Changed SKILL.md files in this pass: **0**


## Numeric-rule scan

The lexical scan found one legitimate governance reference to the phrase “keyword density” in `10_GOVERNANCE/seo-myth-detection/references/hard-rule-audit.md`; it describes the banned rule as a myth to remove and contains no numeric density instruction. No prohibited numeric hard rule is present as an instruction. Fixed title/meta lengths, fixed snippet word counts, and fixed internal-link ratios: **0 actionable occurrences**.


## Outcome framing

README and package text were checked for claims that SuperSEO replaces human SEO expertise or guarantees rankings, traffic, or revenue. No such claims were introduced in this pass.
