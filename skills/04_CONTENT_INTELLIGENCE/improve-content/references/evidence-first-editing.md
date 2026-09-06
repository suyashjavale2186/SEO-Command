# Evidence-First Editing


**Source basis:** Ported and filtered from: skills/improve-content/references/writing-pipeline.md, skills/write-content/references/fact-checking.md. The legacy structure is retained where it is operationally useful; unsupported Google-mechanism claims and arbitrary SEO targets are not carried forward. [Evidence Tier: Tier 3 — Industry observation]


## Ported operating assets


- # Technique 15: Writing Pipeline Architecture [Evidence Tier: Tier 3 — Industry observation]


- ## What It Is [Evidence Tier: Tier 3 — Industry observation]


- A multi-phase, multi-agent pipeline for producing high-quality SEO content. Based on analysis of 15+ agentic writing systems, this architecture represents the consensus best approach: specialized phases with quality gates, not a single monolithic generation. [Evidence Tier: Tier 3 — Industry observation]


- ## Why It Works [Evidence Tier: Tier 3 — Industry observation]


- Research consistently shows that multi-agent pipelines outperform single-prompt generation: [Evidence Tier: Tier 3 — Industry observation]


- - Section-by-section generation maintains quality over long articles [Evidence Tier: Tier 3 — Industry observation]


- - Specialized agents (writer vs. critic) produce better results than a generalist [Evidence Tier: Tier 3 — Industry observation]


- - Iterative revision can improve quality, but the useful stopping rule is evidence and defect reduction rather than a predetermined number of cycles. [Evidence Tier: Tier 2 — Strong empirical evidence]


- - Quality gates prevent bad content from being output [Evidence Tier: Tier 3 — Industry observation]


- Comparisons between human-authored and AI-assisted content vary by study design, audience, and publishing context, so do not use a single multiplier as a planning rule. The actionable requirement is to improve evidence, specificity, usefulness, and editorial judgment. [Evidence Tier: Tier 3 — Industry observation]


- Single-prompt content generation fails because one prompt can't simultaneously optimize for research depth, writing quality, SEO mechanics, anti-detection, and fact accuracy. Each agent focuses on ONE thing well, and each stage builds on verified output from the previous stage. [Evidence Tier: Tier 3 — Industry observation]


- ## The 7-Agent Model [Evidence Tier: Tier 3 — Industry observation]


- The pipeline uses seven specialized agents, each with a distinct role and optimal configuration: [Evidence Tier: Tier 3 — Industry observation]


- ## Implementation Architecture [Evidence Tier: Tier 3 — Industry observation]


- - Article (markdown) [Evidence Tier: Tier 3 — Industry observation]


- - Meta elements [Evidence Tier: Tier 3 — Industry observation]


- - Quality scorecard [Evidence Tier: Tier 3 — Industry observation]


- ## Tips [Evidence Tier: Tier 3 — Industry observation]


## Elite adaptation


The retained pattern should be applied to the real user and business context: Every proposed edit should have a reason tied to observed performance, user need, evidence quality, or business outcome. The reference is a decision aid, not a ranking formula. Start with the observed situation, classify the underlying task or risk, select an intervention that directly addresses it, and define how the result will be validated. [Evidence Tier: Tier 4 — Hypothesis]


Keep observations, interpretations, and hypotheses separate. A current SERP, Search Console row, live HTML response, expert interview, or original dataset is evidence; an explanation of why a proprietary system behaved that way is an interpretation unless officially documented. [Evidence Tier: Tier 1 — Officially documented]


## Execution checklist


1. Confirm scope, affected asset(s), target audience, intended outcome, and available evidence. [Evidence Tier: Tier 4 — Hypothesis]


2. Document the baseline and source provenance before making a change. [Evidence Tier: Tier 2 — Strong empirical evidence]


3. Apply the legacy tactic only where the diagnosed problem calls for it; avoid copying competitors for its own sake. [Evidence Tier: Tier 4 — Hypothesis]


4. Record assumptions and uncertainty, especially where the source material relied on industry inference. [Evidence Tier: Tier 4 — Hypothesis]


5. Validate the implementation and compare the outcome against the same baseline, including business impact when available. [Evidence Tier: Tier 2 — Strong empirical evidence]


## Worked example


Suppose Do not rewrite a page solely because it has been online for a long time. Begin by proving the symptom exists and identifying the page/query/business role involved. If the evidence points to a content problem, add useful information or fix the intent mismatch; if it points to technical access or indexation, fix the underlying technical state first. Do not use a content rewrite to treat a problem whose evidence points elsewhere. [Evidence Tier: Tier 2 — Strong empirical evidence]


## Red flags


## Evidence reminder


Legacy tactical claims are generally **Tier 3 — Industry observation**. Current technical or policy claims should be checked against official Google documentation, and ambiguous claims should default to the weaker tier. [Evidence Tier: Tier 4 — Hypothesis]
