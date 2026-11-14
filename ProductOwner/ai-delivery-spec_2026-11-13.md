---
title: AI Delivery Spec
date: 2026-11-13
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/franklinxkk/ai-delivery-spec
repo: franklinxkk/ai-delivery-spec
status: recommended
---

# AI Delivery Spec

## Verdict

This is worth a product owner's time if the recurring problem is vague requirements turning into rework. It gives an agent a disciplined loop for judging a problem, clarifying scope, writing a handoff-ready requirement, checking prototypes, handling change, and verifying acceptance. It is not a backlog, roadmap, analytics, or team-of-record system, so it should strengthen an existing product workflow rather than pretend to replace one.

## Repository

- Repository: [franklinxkk/ai-delivery-spec](https://github.com/franklinxkk/ai-delivery-spec)
- Primary language: Python
- License: MIT
- Stars: 37
- Forks: 6
- Open issues: 0
- Created: 2026-06-07
- Last pushed: 2026-11-01
- Latest release: [v5.5.6](https://github.com/franklinxkk/ai-delivery-spec/releases/tag/v5.5.6), published 2026-10-31
- Main topics: agent-skills, ai-coding, ai-delivery-spec, claude-skills, codex-skills, coding-agents, cursor, domain-knowledge, prd, product, product-management-skills, product-manager, product-requirements, prototyping, requirements, vibe-coding, workbuddy

## Why This Repo Was Picked

It covers the seam where product work usually breaks: a decision is made, but the rules, boundaries, failure paths, and acceptance evidence are not clear enough for engineering or testing. The repository includes a usable skill, staged references, schemas, scripts, examples, and an interactive review prototype, not just a list of prompts. Recent releases through v5.5.6 show active iteration, and the MIT license keeps reuse straightforward. It beat broader PM skill collections because its core loop is narrow, operational, and tied to delivery handoff.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
| --- | --- | --- |
| [franklinxkk/ai-delivery-spec](https://github.com/franklinxkk/ai-delivery-spec) | Discovery, PRDs, prototypes, change handling, review, and acceptance workflows | Won because it connects product judgment to concrete handoff and verification artifacts |
| [Libres-coder/lifecycle](https://github.com/Libres-coder/lifecycle) | Seven-stage repository checks for discovery through sustainment | Useful but created and pushed on the scan day, with 0 stars and a stronger developer workflow bias |
| [naodeng/dsh-qa](https://github.com/naodeng/dsh-qa) | Local QA workbench for requirements, tests, evidence, defects, and gates | Practical for QA, but tied to DeepSeek Harness and PolyForm Noncommercial licensing |
| [Mehdibargach/claude-code-pm-skills](https://github.com/Mehdibargach/claude-code-pm-skills) | 20 PM commands for discovery, PRDs, roadmaps, metrics, and communication | Broad and easy to browse, but last pushed 2026-03-18 and less explicit about traceable acceptance |
| [OpenRose/OpenRose](https://github.com/OpenRose/OpenRose) | Requirements management application with traceability and baselines | More like a system to deploy and learn than a low-friction workflow a PO can adopt tomorrow |

## What It Is

AI Delivery Spec is an agent skill and supporting toolkit for product discovery, requirements engineering, PRDs, interactive prototypes, change management, and acceptance. It provides four short intent paths: `/dig` for discovery, `/prd` for specification, `/proto` for an interactive prototype, and `/ads` for a broader requirement task. The repository also contains reference guidance, domain-query scripts, JSON schemas, packaging and validation scripts, and example requirement cards, modular PRDs, and review workspaces. It is not a hosted product management application and does not store a team's canonical backlog or roadmap.

## Why It Is Useful For Product Owners

- Backlog refinement: turn a vague ticket into a bounded task with entry conditions, inputs, results, rejected paths, recovery, and explicit non-goals.
- User stories and acceptance criteria: express normal, failure, permission, stale-state, duplicate-request, and empty-result cases instead of stopping at happy-path prose.
- Discovery: challenge whether the proposed feature solves the real problem, compare options, expose unknowns, and preserve decisions that are already authorized.
- Stakeholder alignment: give product, design, engineering, and QA separate reading paths into the same requirement rather than maintaining conflicting summaries.
- Roadmap and prioritization: use the discovery step to record value, cost, risk, and unresolved evidence before a feature is treated as ready for delivery.
- Experimentation: define the target behavior, success evidence, guardrails, and failure interpretation before building an interactive prototype or implementation.
- Delivery coordination: review a change against the current baseline, identify affected modules and consumers, and verify that acceptance evidence still matches the changed requirement.

## How I Would Actually Use It

1. Paste a customer request such as "add automatic approval" into `/dig` and require a problem statement, affected users, alternatives, evidence gaps, and a decision to proceed, narrow, validate, or defer.
2. Run `/prd` on one backlog item and ask for a one-slice handoff covering roles, fields, states, permissions, success results, failure results, recovery, dependencies, and explicit exclusions.
3. Use the example requirement card as a review checklist for a story before refinement: can a developer and tester determine what happens on stale data, duplicate submission, missing permission, and service failure?
4. Give `/proto` an existing page and a confirmed requirement to make a small offline review prototype, then use it to align on interaction behavior without treating the mockup as proof of production behavior.
5. When a stakeholder changes one rule, run the change workflow against the current requirement baseline and record which screens, roles, data states, tests, and acceptance examples are affected.
6. Ask the agent to cold-read the handoff as an independent engineer or tester, then fix gaps it can locate without adding invented policy, permissions, metrics, or defaults.
7. Before marking a feature ready, run the repository's relevant checks and separately confirm real business behavior through the product's actual entry point; keep static checks and human acceptance as distinct evidence.

## Limitations / Watch Outs

- The repository has modest adoption evidence: 37 stars and 6 forks do not prove that teams get better product outcomes.
- The README and much of the detailed guidance are Chinese-first. The English section is useful for orientation, but teams may need to translate or adapt deeper references.
- It requires an agent host that supports skills. The one-minute install uses `npx skills add`, and deeper workflows may use Python scripts and local project files.
- It is not a Jira, Linear, Azure DevOps, analytics, research repository, or release-management system. Outputs still need to be copied into the team's system of record.
- Generated requirements can sound rigorous while encoding unsupported assumptions. The repository itself warns that examples are not project facts and that structure passing does not prove business correctness.
- Prototype review is not production acceptance. A simulated browser flow can miss authentication, data integrity, concurrency, instrumentation, accessibility, or operational behavior.
- The repository is maintained actively but has a relatively young history and no open issues at scan time. Teams should pin a release and recheck upgrade behavior before standardizing it.

## Best Starting Points

- [README](https://github.com/franklinxkk/ai-delivery-spec/blob/main/README.md)
- [Skill definition](https://github.com/franklinxkk/ai-delivery-spec/blob/main/SKILL.md)
- [Minimal requirement card example](https://github.com/franklinxkk/ai-delivery-spec/blob/main/examples/minimal-v5/requirement-card.md)
- [Modular PRD example](https://github.com/franklinxkk/ai-delivery-spec/blob/main/examples/medium-review-handoff/requirement.md)
- [Interactive review prototype](https://github.com/franklinxkk/ai-delivery-spec/blob/main/examples/medium-review-handoff/review-prototype.html)
- [Review workspace guidance](https://github.com/franklinxkk/ai-delivery-spec/blob/main/references/review-workspace.md)
- [Latest release](https://github.com/franklinxkk/ai-delivery-spec/releases/tag/v5.5.6)

## Metadata

- Scan date: 2026-11-13
- Canonical repository URL: https://github.com/franklinxkk/ai-delivery-spec
- Duplicate detection uses the canonical GitHub repository URL, normalized by owner and repository name, across all Markdown files in the vault.
