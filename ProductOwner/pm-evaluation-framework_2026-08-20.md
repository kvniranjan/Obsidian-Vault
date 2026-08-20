---
title: pm-evaluation-framework
date: 2026-08-20
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/kalyvask/pm-evaluation-framework
repo: kalyvask/pm-evaluation-framework
status: recommended
---

# pm-evaluation-framework

## Verdict
This is worth a product owner's time if they want sharper PM artifacts and decision discipline, not another task tracker. The repo is light on community proof, with 0 stars and 0 forks at scan time, so do not treat it as a battle-tested standard. Still, the actual contents are practical: PRD and decision templates, prioritization guidance, review rubrics, lifecycle frameworks, and PM-focused agent skills.

## Repository
- Repository: [https://github.com/kalyvask/pm-evaluation-framework](https://github.com/kalyvask/pm-evaluation-framework)
- Owner/repo: `kalyvask/pm-evaluation-framework`
- Primary language: Go Template
- License: MIT
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-05-05
- Last pushed: 2026-08-16
- Latest release: [v1.0.0](https://github.com/kalyvask/pm-evaluation-framework/releases/tag/v1.0.0), published 2026-06-10
- Main topics: ai-pm, claude-code, claude-skills, decision-frameworks, frameworks, mba, pm, pm-frameworks, pmf, product-management, product-market-fit, product-strategy, rubrics, skills

## Why This Repo Was Picked
It won because it has reusable product work assets, not just reading material. The strongest parts are the PRD template, decision memo and decision log templates, launch criteria, PM prompt library, prioritization guidance, metrics guidance, stakeholder alignment material, and three review rubrics. It also has 23 lifecycle-oriented Claude Code skills, which are not directly Codex-ready, but the underlying instructions can still be mined for PO workflows.

The tradeoff is obvious: adoption signal is weak. I picked it anyway because the content is more immediately applicable to backlog refinement, prioritization, PRD review, launch readiness, stakeholder alignment, and metrics conversations than the noisier high-update repos in the scan.

## Shortlist Considered
| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [kalyvask/pm-evaluation-framework](https://github.com/kalyvask/pm-evaluation-framework) | PM templates, rubrics, lifecycle frameworks, decision docs, and 23 PM agent skills | Won because it is broad, inspectable, recently pushed, MIT licensed, and usable for real PO artifacts |
| [PANGKAIFENG/ai-product-manager-skills](https://github.com/PANGKAIFENG/ai-product-manager-skills) | Codex/Claude-oriented PM skills for research, PRD work, requirements review, and delivery loops | Strong but Chinese-first, more runtime-skill focused, and less immediately readable for an English PO vault memo |
| [CaufieldZ/pm-workspace-public](https://github.com/CaufieldZ/pm-workspace-public) | AI-native PM workspace with examples, PRD pipeline, setup docs, and Claude skills | Substantial but heavier setup and more Claude/workspace-specific than a reusable PO reference |
| [Sofeso/accessibility-acceptance-criteria-toolkit](https://github.com/Sofeso/accessibility-acceptance-criteria-toolkit) | WCAG 2.2 acceptance criteria, accessibility defect template, and inclusive user stories | Useful but too narrow for the one daily pick |
| [hi0001234d/nexpath](https://github.com/hi0001234d/nexpath) | Local-first AI coding workflow for product managers and technical founders | More engineering quality workflow than day-to-day PO operating artifact |

## What It Is
This is a documentation and agent-skill repository for product management practice. It contains lifecycle frameworks, decision-making guides, artifact templates, evaluation rubrics, a PM prompt library, and Claude Code skills organized around PM activities. It is not a product management app, backlog system, or analytics platform.

Useful folders and files include:
- `templates/` for PRD, decision memo, decision log, launch criteria, postmortem, and prompt library assets.
- `rubrics/` for PM evaluation, product review, and strategy memo review.
- `decision-making/` for prioritization, metrics, customer interviews, AI integration, value hypotheses, activation, conversion, and related decisions.
- `frameworks/` for discovery, MVP, PMF, growth, and continuous prioritization.
- `.claude/skills/` for PM workflow skills that can be adapted into prompts or Codex skills.

## Why It Is Useful For Product Owners
For backlog refinement, the PRD template forces a clear user, job, blocker, cost, out-of-scope list, tradeoffs, success criteria, risks, reversibility, open questions, dependencies, and implementation milestones.

For prioritization, the repo gives a working language for separating strategic problem choice from tactical feature ordering, then uses painkiller versus vitamin, toothbrush test, Severity x Frequency x Feasibility, RICE, WSJF, and MoSCoW.

For discovery, it includes customer interview and value hypothesis material that can prevent a PO from turning stakeholder requests into backlog items without evidence.

For stakeholder alignment, it has decision memo, decision log, progress audit, product review, and strategy memo review assets that make disagreement visible before delivery starts.

For delivery coordination, the launch criteria and postmortem templates help turn "ready" and "done" into reviewable criteria instead of vibes.

## How I Would Actually Use It
1. Copy the PRD template into a feature intake note and fill only the sections that change the decision: problem, why now, out of scope, success criteria, risks, reversibility, and dependencies.
2. Use the prioritization guide before sprint planning to separate "which problem matters" from "which solution goes first."
3. Run a stakeholder request through the decision memo template before escalating it, especially when the request competes with committed roadmap work.
4. Use the product review rubric as a pre-read checklist before a roadmap or feature review.
5. Use the metrics material to define a primary metric, guardrails, failure threshold, and acceptable learning range before delivery starts.
6. Mine the `.claude/skills/pm-progress-auditor` and `.claude/skills/pm-red-team` instructions as prompt material for reviewing status updates and high-stakes product memos.
7. Use the launch criteria template to create a release gate for risky features, including operational readiness and rollback expectations.

## Limitations / Watch Outs
- Community signal is weak: 0 stars and 0 forks at scan time. That means you are judging the content yourself.
- The skills are Claude Code oriented. They are useful as source material, but they are not drop-in Codex skills without adaptation.
- Some material is framework-heavy. A PO can waste time reading if they do not start from a live artifact or decision.
- The repo is not a system of record. It will not replace Jira, Linear, Productboard, analytics, or research repositories.
- The value depends on disciplined use. Templates will not fix vague strategy, weak discovery, or missing stakeholder ownership.

## Best Starting Points
- [README](https://github.com/kalyvask/pm-evaluation-framework/blob/main/README.md)
- [Templates folder](https://github.com/kalyvask/pm-evaluation-framework/tree/main/templates)
- [PRD template](https://github.com/kalyvask/pm-evaluation-framework/blob/main/templates/prd-template.md)
- [Decision memo template](https://github.com/kalyvask/pm-evaluation-framework/blob/main/templates/decision-memo.md)
- [Launch criteria template](https://github.com/kalyvask/pm-evaluation-framework/blob/main/templates/launch-criteria.md)
- [Prioritization guide](https://github.com/kalyvask/pm-evaluation-framework/blob/main/decision-making/prioritization.md)
- [Metrics guide](https://github.com/kalyvask/pm-evaluation-framework/blob/main/decision-making/metrics.md)
- [Rubrics folder](https://github.com/kalyvask/pm-evaluation-framework/tree/main/rubrics)
- [Claude skills folder](https://github.com/kalyvask/pm-evaluation-framework/tree/main/.claude/skills)
- [Latest release v1.0.0](https://github.com/kalyvask/pm-evaluation-framework/releases/tag/v1.0.0)

## Metadata
- Scan date: 2026-08-20
- Canonical repository URL: https://github.com/kalyvask/pm-evaluation-framework
- Duplicate detection: uses the canonical GitHub repository URL as the unique key across Markdown file contents, including shortlist tables.
