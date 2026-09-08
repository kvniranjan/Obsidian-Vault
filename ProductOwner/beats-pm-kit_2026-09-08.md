---
title: beats-pm-kit
date: 2026-09-08
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/officebeats/beats-pm-kit
repo: officebeats/beats-pm-kit
status: recommended
---

# beats-pm-kit

## Verdict

Beats PM Kit is worth a product owner's time if product context is scattered across meetings, chat, documents, and task lists. It is a runnable local-first PM operating harness with evidence intake, discovery, prioritization, tracking, communication, and Codex or Obsidian adapters, not another prompt dump. The catch is serious: there is no declared license, the setup is substantial, and the repository is complex enough to require an owner who will maintain the workflow.

## Repository

- Repository: [officebeats/beats-pm-kit](https://github.com/officebeats/beats-pm-kit)
- Primary language: Python
- License: no GitHub license metadata and no `LICENSE` file found at the repository root during this scan
- Stars: 9
- Forks: 1
- Open issues: 0
- Created: 2025-12-28
- Last pushed: 2026-08-27
- Main topics: `ai-agents`, `notion`, `obsidian`, `pm-tools`, `product-management`, `productivity`, `project-management`, `second-brain`
- Latest release: [v14.0.0](https://github.com/officebeats/beats-pm-kit/releases/tag/v14.0.0), published 2026-08-27

## Why This Repo Was Picked

This repo won because it connects evidence capture to actual product work. It has canonical local Markdown state, bounded context retrieval, task ledgers, discovery, prioritization, sprint and retrospective workflows, stakeholder communication, and explicit Codex and Obsidian runtime support. That is more useful for day-to-day PO work than another static PRD template or a narrowly scoped feedback board. Recent release activity is meaningful, but the low star count and missing license keep this at "inspect and pilot," not "adopt blindly."

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
| --- | --- | --- |
| [officebeats/beats-pm-kit](https://github.com/officebeats/beats-pm-kit) | Local-first PM harness with evidence, workflows, task state, runtime adapters, and Obsidian support | Won because it covers the full operating loop and matches this vault's Markdown workflow |
| [bymilon/factoryos](https://github.com/bymilon/factoryos) | Spec-driven software factory with plans, tasks, validation, and Codex commands | Strong engineering handoff tool, but narrower than daily PO discovery, stakeholder, and evidence work |
| [yohayetsion/product-org-os](https://github.com/yohayetsion/product-org-os) | Agent-based product organization with skills, templates, and product gateway commands | Too new to trust yet: created and pushed 2026-09-07 with 0 stars and 0 forks |
| [product-on-purpose/product-lifecycle-templates](https://github.com/product-on-purpose/product-lifecycle-templates) | Governed Markdown bundles for PRDs, stories, backlogs, risks, KPIs, and decisions | Already covered in the vault and is a template library, not an operating harness |
| [agentmart/pm-os](https://github.com/agentmart/pm-os) | Claude Code and Copilot PM OS with routines, templates, and quality hooks | Already covered in the vault and more runtime-specific than the selected repo |

## What It Is

Beats PM Kit is a local-first, cross-runtime product-management harness. It provides a numbered Markdown workspace for company context, products, meetings, people, trackers, resources, SOPs, partners, and clients; an `.agent/` contract for rules, skills, workflows, and command routing; generated adapters for Codex, Claude, Gemini, Copilot, and Obsidian; and Python utilities for task intake, vault queries, context retrieval, transcript processing, privacy checks, and upgrade compatibility.

It is software plus workflow content, not a hosted backlog product. The repository expects the team to clone it, bootstrap a local workspace, and operate from human-readable Markdown task notes while generated navigation and runtime adapters remain derived views.

## Why It Is Useful For Product Owners

- Backlog refinement: use `/track` and canonical task notes to preserve evidence, decisions, dependencies, owners, and progress instead of flattening everything into a task list.
- Discovery: use `/discover` to frame outcomes, map opportunities, rank assumptions by certainty and criticality, and design the cheapest validation experiment.
- Prioritization: use `/prioritize` with RICE, ICE, MoSCoW, Kano, or weighted scoring, then document the cut line and capacity check.
- Requirements: use `/create`, the PRD authoring skills, and product folders to turn evidence into briefs, PRDs, epics, and stories.
- Stakeholder alignment: use `/meet`, `/prep`, `/boss`, `/review`, and `/week` to convert meeting evidence into decisions, follow-ups, and readable updates.
- Delivery coordination: use `/sprint`, `/retro`, `/handoff`, and `/day` to keep commitments, risks, and next actions visible without making a second system of record.
- Governance: use bounded retrieval, source links, privacy guards, and human approval rules to reduce fabricated context and accidental leakage from local PM material.

## How I Would Actually Use It

1. Clone the repository into a pilot folder and run the non-interactive bootstrap, then inspect the generated `AGENTS.md`, `CODEX_COMMANDS.md`, and local workspace layout before importing any sensitive material.
2. Put one real product's company context, current PRD, recent meeting notes, and backlog signals into the numbered folders, keeping raw evidence separate from derived summaries.
3. Run `/meet` or `/transcript` on one recent planning session, then verify that the resulting decisions and tasks link back to the source evidence.
4. Run `/discover` for one disputed initiative and require the output to name the business outcome, riskiest assumption, cheapest experiment, owner, and decision gate.
5. Run `/prioritize` on a deliberately small backlog, compare its recommendation with the team's existing ranking, and record where evidence or capacity changes the order.
6. Use `/week` and `/review` to produce a stakeholder update from canonical task notes, then check that no private source content is promoted beyond the intended workspace.

## Limitations / Watch Outs

- No declared license was found. Do not treat this as safe for commercial redistribution or internal legal approval until the maintainer clarifies licensing.
- Adoption proof is weak: 9 stars and 1 fork do not establish a durable community or support path.
- The setup is not lightweight. Bootstrap, generated adapters, local workspace conventions, optional hooks, and upgrade compatibility create ongoing maintenance work.
- It is not a replacement for Jira, Linear, Azure DevOps, or a dedicated analytics platform. Integrations and source connectors still need configuration and may be organization-specific.
- The repository is broad and can become process theater. Start with one product, one evidence lane, and a few workflows; do not import every skill and folder at once.
- The README says private material stays local, but the selected AI runtime still processes prompts and tool outputs. Privacy depends on runtime settings and operator discipline.
- The repository is actively evolving, so generated files and command names may change between releases. Pin a release before a team pilot.

## Best Starting Points

- [README](https://github.com/officebeats/beats-pm-kit#readme): scope, setup, workspace model, workflows, and privacy posture
- [Getting started in the repository](https://github.com/officebeats/beats-pm-kit): begin with `install.sh` or `python3 system/scripts/bootstrap.py --agent --non-interactive`
- [Codex command table](https://github.com/officebeats/beats-pm-kit/blob/main/CODEX_COMMANDS.md): full routed command inventory and runtime promotion status
- [Discovery workflow](https://github.com/officebeats/beats-pm-kit/blob/main/.agent/workflows/discover.md): outcome, assumptions, experiments, and stakeholder gate
- [Prioritization workflow](https://github.com/officebeats/beats-pm-kit/blob/main/.agent/workflows/prioritize.md): framework selection, scoring, capacity, and cut line
- [Tracking workflow](https://github.com/officebeats/beats-pm-kit/blob/main/.agent/workflows/track.md): evidence handling, canonical task notes, and navigation rebuilds
- [Runtime compatibility](https://github.com/officebeats/beats-pm-kit/blob/main/system/docs/runtime-compatibility.md): Codex, Claude, Gemini, Copilot, and adapter boundaries
- [Latest release](https://github.com/officebeats/beats-pm-kit/releases/tag/v14.0.0): pin this version for an initial pilot

## Metadata

- Scan date: 2026-09-08
- Canonical repository URL: https://github.com/officebeats/beats-pm-kit
- Duplicate detection uses the canonical GitHub repository URL across all Markdown files in the vault, not filenames or note titles.
