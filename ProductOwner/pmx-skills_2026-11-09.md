---
title: pmx-skills
date: 2026-11-09
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/pskoett/pmx-skills
repo: pskoett/pmx-skills
status: recommended
---

# pmx-skills

## Verdict

PMX-Skills is worth a product owner's time if recurring product decisions are being made from scattered context, weak evidence, or undocumented assumptions. It gives an agent concrete workflows for weekly prioritization, feedback triage, OKR review, planning interviews, decision logs, and business reviews. It is not a mature product platform: adoption is tiny, maintenance has been quiet since September 2026, and the outputs still depend on the quality of the context you provide.

## Repository

- Repository: [pskoett/pmx-skills](https://github.com/pskoett/pmx-skills)
- Owner/repo: `pskoett/pmx-skills`
- Primary language: Python
- License: MIT
- Stars: 3
- Forks: 1
- Open issues: 0
- Created date: 2026-09-06
- Last pushed date: 2026-09-16
- Main topics: None listed
- Releases: None found

## Why This Repo Was Picked

PMX-Skills won because it is a compact operating layer for actual PO work rather than another broad prompt dump or static reading list. Its bundled workflows cover prioritization, customer-feedback synthesis, OKR confidence, planning interviews, decision provenance, stakeholder context, and review artifacts. The repository also states clear boundaries: examples and evaluations are synthetic, personal and customer data should stay in a controlled workspace, and the skills should be adapted to local decision logic.

It has low setup burden because the skills are plain Markdown under `.agents/skills/`, with an optional Agent Plugins package and Claude Code plugin. That makes a one-workflow pilot realistic even though the repository's community and maintenance signals are weak.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [pskoett/pmx-skills](https://github.com/pskoett/pmx-skills) | Context-first PM skills for prioritization, feedback triage, OKRs, planning, decisions, reviews, and knowledge curation | Won because it covers recurring PO operating work with low setup and inspectable Markdown workflows |
| [sriramgopalan/opencan](https://github.com/sriramgopalan/opencan) | Self-hosted feedback boards, voting, roadmap, changelog, webhooks, and embeddable widget | Practical, but requires Docker, PostgreSQL, Redis, OAuth, and email configuration; too much infrastructure for this scan |
| [ombharatiya/AI-for-Product-Managers](https://github.com/ombharatiya/AI-for-Product-Managers) | Large AI PM learning guide with product craft, evals, metrics, case studies, and interview material | Useful reference, but primarily a curriculum and knowledge base, not a day-to-day operating workflow |
| [menkesu/awesome-pm-skills](https://github.com/menkesu/awesome-pm-skills) | 25 PM workflows for discovery, strategy, specs, prioritization, experiments, and launches | Already covered in the vault; PMX-Skills adds a smaller context-management and operating-rhythm angle rather than duplicating its broad skill catalog |
| [davidjwhenry/productownertoolkit](https://github.com/davidjwhenry/productownertoolkit) | Markdown-first PO workflow for research, PRDs, backlog work, UAT, prototypes, and stakeholder reports | Already covered in the prior scan; broader lifecycle coverage, but heavier than the focused recurring-decision pilot selected here |

## What It Is

PMX-Skills is a plain-Markdown AI skill library and Agent Plugins package for product management. It is not a backlog database, roadmap application, analytics platform, or system of record. The bundled skills provide procedures, prompts, references, and evaluation scenarios that an agent can run against product context stored in an appropriate workspace.

The repository includes 13 bundled skills, including first-principles thinking, ghost writing, weekly prioritization, feedback triage, OKR coaching, business reviews, team context updates, knowledge-base curation, decision logs, visualization critique, product-planning interviews, HTML artifacts, and discovery of optional companion skills. The package also documents optional Claude Code and portable Agent Plugins installation paths.

## Why It Is Useful For Product Owners

- Backlog refinement: use `weekly-prioritization` to reconcile goals, evidence, capacity, and active work before changing priority order.
- Discovery: use `product-planning-interview` to expose needs, boundaries, risks, and success criteria before asking for a plan.
- Feedback analysis: use `feedback-triage` to group customer input into traceable needs and propose proportionate actions instead of counting requests blindly.
- Stakeholder alignment: use `team-context-update` and `business-review` to separate context, outcomes, risks, learning, and next-period decisions from the delivery board.
- Metrics and goals: use `okr-coach` to test whether results are measured, confidence is explicit, and the next action follows from evidence.
- Decision quality: use `first-principle-thinking` and `decision-log` to challenge solution assumptions and preserve rationale, consequences, and provenance.
- Delivery coordination: use `knowledge-base-curator` to keep a source-backed Markdown context layer that can be reused across refinement, planning, and reviews.

## How I Would Actually Use It

1. Install only `weekly-prioritization` and `decision-log`, then run a Friday review using the current goals, capacity, active work, and evidence links.
2. Feed the last month of support tickets and interview notes to `feedback-triage`; review its themes and reject any recommendation that cannot point back to source evidence.
3. Before opening an epic, run `product-planning-interview` to produce explicit users, problem boundaries, risks, and success criteria for the engineering conversation.
4. Run `okr-coach` on a monthly metric review and record confidence, missing measurement, and the smallest corrective action in the decision log.
5. Use `first-principle-thinking` when a stakeholder requests a feature, forcing the team to test the problem, constraint, and cheapest falsifying experiment before committing scope.
6. Use `business-review` to turn delivery results, customer learning, risks, and next-period decisions into a concise stakeholder review rather than a status dump.
7. Keep generated artifacts in a controlled product workspace, with links to the source notes and a human owner responsible for approving the final decision.

## Limitations / Watch Outs

- Community proof is weak: 3 stars, 1 fork, no open issues, and no releases do not establish adoption or long-term support.
- The last push was 2026-09-16, so the repository may already be stale for a fast-moving agent ecosystem.
- It does not connect to Jira, Linear, GitHub Projects, analytics, CRM, or customer-support systems. Copying context into files is still a manual step.
- The workflows produce recommendations and artifacts, not validated product decisions. An agent can summarize bad evidence convincingly.
- The repository's examples and evaluation scenarios are synthetic. They demonstrate workflow shape, not production effectiveness.
- Installing all 13 skills at once creates choice overload and can make routing less predictable. Start with one or two recurring workflows.
- The optional plugin formats add client-specific installation rules, and symlink handling can complicate packaging on some systems.
- Personal profiles, customer records, and proprietary product knowledge must not be placed in the shared repository.

## Best Starting Points

- [README](https://github.com/pskoett/pmx-skills#readme)
- [Weekly prioritization skill](https://github.com/pskoett/pmx-skills/tree/main/.agents/skills/weekly-prioritization)
- [Feedback triage skill](https://github.com/pskoett/pmx-skills/tree/main/.agents/skills/feedback-triage)
- [Product planning interview skill](https://github.com/pskoett/pmx-skills/tree/main/.agents/skills/product-planning-interview)
- [Decision log skill](https://github.com/pskoett/pmx-skills/tree/main/.agents/skills/decision-log)
- [OKR coach skill](https://github.com/pskoett/pmx-skills/tree/main/.agents/skills/okr-coach)
- [Plugin manifest](https://github.com/pskoett/pmx-skills/blob/main/plugin.json)

## Metadata

- Scan date: 2026-11-09
- Canonical repository URL: https://github.com/pskoett/pmx-skills
- Duplicate detection uses the canonical GitHub repository URL across every Markdown file in the Obsidian vault.
