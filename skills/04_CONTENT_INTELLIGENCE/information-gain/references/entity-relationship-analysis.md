# Entity Relationship Analysis


**Source basis:** Ported and filtered from: skills/semantic-gap-analysis/references/eav-triple-worked-examples.md, skills/semantic-gap-analysis/references/predicate-verb-fields.md. The legacy structure is retained where it is operationally useful; unsupported Google-mechanism claims and arbitrary SEO targets are not carried forward. [Evidence Tier: Tier 3 — Industry observation]


## Ported operating assets


- # EAV Triple Worked Examples [Evidence Tier: Tier 3 — Industry observation]


- EAV modeling is hard to learn abstractly. What follows is a set of worked examples across domains — each one showing the thin-keyword version of a topic alongside the rich semantic version a domain expert would write. The contrast is the point. When you run Step 5 of the skill (Map Entity Relationships), these are the shapes you're aiming for. [Evidence Tier: Tier 3 — Industry observation]


- The framework is Koray Tuğberk GÜBÜR's: every entity on a page should carry attributes and relations to other entities in the same topic space. Subject, predicate, object. A page that lists entities without attributes reads to a language model the same way a glossary reads to a human — flat. A page with EAV coverage reads like someone who actually knows the topic. [Evidence Tier: Tier 3 — Industry observation]


- ## Example 1 — Espresso machines [Evidence Tier: Tier 3 — Industry observation]


> espresso machine, coffee machine, best espresso machine, $5000 espresso machine, commercial espresso machine [Evidence Tier: Tier 3 — Industry observation]


- - **Entity:** La Marzocco Linea Mini [Evidence Tier: Tier 3 — Industry observation]


- - **Attributes:** brew pressure (9 bar), boiler configuration (dual boiler, saturated group), price point (~EUR 5,800), heat-up time (~20 min), PID temperature stability (±0.5°C), E61-derived group head with saturated design [Evidence Tier: Tier 3 — Industry observation]


- ## Cross-reference [Evidence Tier: Tier 3 — Industry observation]


## Elite adaptation


The retained pattern should be applied to the real user and business context: Represent important entities as subject–predicate–object or attribute relationships and inspect whether the page explains the relationships readers need. The reference is a decision aid, not a ranking formula. Start with the observed situation, classify the underlying task or risk, select an intervention that directly addresses it, and define how the result will be validated. [Evidence Tier: Tier 4 — Hypothesis]


Keep observations, interpretations, and hypotheses separate. A current SERP, Search Console row, live HTML response, expert interview, or original dataset is evidence; an explanation of why a proprietary system behaved that way is an interpretation unless officially documented. [Evidence Tier: Tier 1 — Officially documented]


## Execution checklist


1. Confirm scope, affected asset(s), target audience, intended outcome, and available evidence. [Evidence Tier: Tier 4 — Hypothesis]


2. Document the baseline and source provenance before making a change. [Evidence Tier: Tier 2 — Strong empirical evidence]


3. Apply the legacy tactic only where the diagnosed problem calls for it; avoid copying competitors for its own sake. [Evidence Tier: Tier 4 — Hypothesis]


4. Record assumptions and uncertainty, especially where the source material relied on industry inference. [Evidence Tier: Tier 4 — Hypothesis]


5. Validate the implementation and compare the outcome against the same baseline, including business impact when available. [Evidence Tier: Tier 2 — Strong empirical evidence]


## Worked example


Suppose For a CRM article, model CRM → integrates with → accounting platform, and then explain setup conditions and limitations. Begin by proving the symptom exists and identifying the page/query/business role involved. If the evidence points to a content problem, add useful information or fix the intent mismatch; if it points to technical access or indexation, fix the underlying technical state first. Do not use a content rewrite to treat a problem whose evidence points elsewhere. [Evidence Tier: Tier 2 — Strong empirical evidence]


## Red flags


- A source claims that an action guarantees rankings, traffic, links, snippets, or AI citations. Treat that as unsupported unless the evidence actually establishes it. [Evidence Tier: Tier 4 — Hypothesis]
- A tactic uses arbitrary density, title/meta length, snippet-length, or internal-link-ratio targets as requirements. Replace them with qualitative objectives. [Evidence Tier: Tier 1 — Officially documented]
- A recommendation cites a proprietary Google mechanism as fact. Downgrade it to Tier 4 — Hypothesis or omit the mechanism entirely. [Evidence Tier: Tier 4 — Hypothesis]
- The proposed content includes invented experience, credentials, customer results, or proprietary measurements. Stop and request verifiable evidence. [Evidence Tier: Tier 1 — Officially documented]


## Evidence reminder


Legacy tactical claims are generally **Tier 3 — Industry observation**. Current technical or policy claims should be checked against official Google documentation, and ambiguous claims should default to the weaker tier. [Evidence Tier: Tier 4 — Hypothesis]
