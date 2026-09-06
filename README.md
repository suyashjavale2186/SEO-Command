# SuperSEO Elite

**An evidence-driven SEO research, strategy, drafting, and measurement co-pilot for human SEO practitioners.**

![Version](https://img.shields.io/badge/version-4.0-blue)
![Skills](https://img.shields.io/badge/skills-44-brightgreen)
![License](https://img.shields.io/badge/license-Apache%202.0-lightgrey)
![Built for](https://img.shields.io/badge/built%20for-Claude-orange)

---

## Table of Contents

- [What This Is](#what-this-is)
- [Why It Exists](#why-it-exists)
- [Architecture](#architecture)
- [The Evidence-Tier System](#the-evidence-tier-system)
- [Installation](#installation)
- [Folder Structure](#folder-structure)
- [Limitations](#limitations)
- [Changelog](#changelog)
- [Credits](#credits)
- [License](#license)

---

## What This Is

SuperSEO Elite is a structured skill system for Claude that supports SEO research, strategy, content briefing, drafting, and performance measurement. It's built to be used *by* a practitioner, not *instead of* one.

It does not have live-site access, doesn't manage client relationships, and doesn't carry accountability for outcomes. Every recommendation it produces is meant to be reviewed by a human before it's acted on, and nothing in this system promises rankings, traffic, or revenue results.

## Why It Exists

Most AI SEO tooling states best-practice numbers — keyword density targets, exact title-character limits, fixed snippet word counts — as if they were Google's actual rules. They usually aren't. They're heuristics, folklore, or outdated advice presented with false confidence.

SuperSEO Elite is built around the opposite habit: **every non-trivial claim is tagged with how well-supported it actually is**, and fixed numeric "rules" that Google doesn't document are deliberately excluded in favor of qualitative judgment grounded in the live SERP, the site's own data, and the practitioner's context. A dedicated Governance layer (`10_GOVERNANCE`) exists specifically to catch overconfident or unsupported claims before they reach an output.

## Architecture

SuperSEO Elite is organized into 10 categories, each responsible for a distinct part of the SEO operating loop — from understanding the business, through research and content, to execution, measurement, and self-correction.

| # | Category | Responsible for |
|---|---|---|
| 01 | **Business Intelligence** | Grounding SEO work in real business context, audience needs, and conversion definitions — not rankings for their own sake |
| 02 | **Site Intelligence** | Technical audits, site structure, internal linking, cannibalization, and indexation diagnostics |
| 03 | **Search Intelligence** | Keyword opportunity, live SERP analysis, intent inference, competitor analysis, and generative-search visibility |
| 04 | **Content Intelligence** | Content briefs, information-gain analysis, E-E-A-T review, expert-interview extraction, drafting, and content improvement |
| 05 | **Authority** | Legitimate link opportunities, digital PR, and authority-evidence evaluation — with manipulative tactics explicitly filtered out |
| 06 | **Execution** | Turning diagnoses into implementation-ready technical fixes, content decisions, link actions, and publishing sequences |
| 07 | **Measurement** | Search Console and analytics interpretation, conversion tracking, content decay detection, and generative-search measurement |
| 08 | **Experimentation** | Structured hypotheses, experiment design, measurement rigor, and a durable learning log |
| 09 | **Strategy** | Business-aware opportunity scoring, prioritization, and roadmap sequencing |
| 10 | **Governance** | Evidence classification, fact-checking, red-teaming, risk detection, and SEO-myth detection — the layer that keeps everything else honest |

Each category contains multiple skills (44 in total); the full list is in [`skills/`](./skills) and declared in [`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json).

## The Evidence-Tier System

Every skill that produces a recommendation classifies its supporting evidence into one of four tiers:

| Tier | Meaning |
|---|---|
| **1 — Official** | Documented directly in Google Search Central / Search Essentials or another primary source |
| **2 — Empirical** | Backed by a large-scale, reproducible independent study |
| **3 — Observational** | Consistent industry observation (e.g. Ahrefs, Semrush, credible case studies) without controlled proof |
| **4 — Hypothesis** | A plausible interpretation with no strong causal evidence — treated as a hypothesis, not a rule |

Recommendation-producing skills follow a consistent output format so a practitioner can see exactly how confident a claim is and what it would cost to act on it:

```text
Recommendation: <what to do>
Evidence: <what supports it>
Confidence: <percentage or High / Medium / Low>
Expected impact: <Low / Medium / High>
Risk: <Low / Medium / High>
Effort: <Low / Medium / High>
Priority: <P1 / P2 / P3>
Evidence status: <Official / Empirical / Observational / Hypothesis>
```

This is what lets `10_GOVERNANCE/seo-myth-detection` and `10_GOVERNANCE/red-team` catch a claim before it's acted on — rather than a confident-sounding tactic being treated as fact just because it's phrased like one.

## Installation

SuperSEO Elite is packaged as a Claude plugin, declared in [`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json) and [`.claude-plugin/marketplace.json`](./.claude-plugin/marketplace.json). The general pattern for installing a Claude plugin from a marketplace manifest is to add this repository as a plugin source and enable it from your Claude environment's plugin/skill settings.

> **Note:** the exact install command and UI may differ depending on which Claude surface you're using (Claude Code, Claude Desktop, Claude.ai). Verify the current steps against [Claude's plugin documentation](https://docs.claude.com) before installing, rather than relying solely on this README.

Once installed, individual skills activate automatically when a request matches their trigger conditions (defined in each skill's `SKILL.md`) — there's no need to invoke them by name.

## Folder Structure

```text
superseo-elite/
├── .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── README.md
├── CHANGELOG.md
├── LICENSE
├── NOTICE
├── SECURITY.md
├── CONTRIBUTING.md
└── skills/
    ├── 01_BUSINESS_INTELLIGENCE/   (business-context, audience-model, conversion-model)
    ├── 02_SITE_INTELLIGENCE/       (technical-seo-audit, site-graph, internal-links, cannibalization, indexation)
    ├── 03_SEARCH_INTELLIGENCE/     (keyword-opportunity, serp-analysis, intent-analysis, competitor-analysis, generative-search, serp-feature-optimization)
    ├── 04_CONTENT_INTELLIGENCE/    (content-brief, information-gain, eeat, expert-interview, write-content, improve-content)
    ├── 05_AUTHORITY/               (digital-pr, link-opportunities, authority-analysis)
    ├── 06_EXECUTION/               (technical-fixes, content-updates, internal-link-actions, publishing-plan)
    ├── 07_MEASUREMENT/             (search-console-analysis, analytics-analysis, conversions, generative-search-visibility, content-decay)
    ├── 08_EXPERIMENTATION/         (hypothesis, seo-experiment, measurement, learning)
    ├── 09_STRATEGY/                (opportunity-scoring, prioritization, seo-roadmap)
    └── 10_GOVERNANCE/              (evidence-engine, fact-checking, red-team, risk-detection, seo-myth-detection)
```

Each skill folder contains a `SKILL.md` (its workflow and output format) and a `references/` folder (supporting tactical and methodological detail).

## Limitations

- **No live-site access.** It can't crawl your site, pull your actual Search Console data, or verify a claim against your real analytics — those still need to be connected or supplied.
- **No outcome guarantees.** Nothing here promises rankings, traffic, or revenue. Evidence tiers describe confidence in a *claim*, not a guarantee of *results*.
- **Not a replacement for technical tooling.** Google Search Console, GA4, and a real crawler (e.g. Screaming Frog) remain necessary for technical SEO work — this system reasons about that data, it doesn't generate it.
- **Requires practitioner review.** Every recommendation is meant to be checked by a human who understands the specific site and business before it's implemented.

## Changelog

See [`CHANGELOG.md`](./CHANGELOG.md) for the full version history, including the four-iteration rebuild from the original SuperSEO plugin.

## Credits

**Created and architected by SUYASH JAVALE.**

Suyash designed the evidence-tier governance system, defined the 10-category skill architecture, and directed the full rebuild of this plugin across four iterations — from the original SuperSEO plugin through the removal of unsupported numeric SEO rules, the addition of the governance and experimentation layers, and the final de-duplication and depth pass.

<!-- add contact / GitHub / portfolio link here -->
[Suyash](#)

## License

Licensed under Apache License 2.0 — see [`LICENSE`](./LICENSE) for full terms.
