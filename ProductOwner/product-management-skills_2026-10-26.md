---
title: product-management-skills
date: 2026-10-26
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/jpoindexter/product-management-skills
repo: jpoindexter/product-management-skills
status: recommended
---

# product-management-skills

## Verdict

This is worth a product owner's time if the team already uses Codex or Claude and wants repeatable decision workflows instead of improvised prompts. The repo is small and has only 1 star, so its quality is not community-proven, but its `/pm` router and explicit output contracts make it more operational than a generic PM prompt collection. Treat it as a workflow starter that needs local review, not as an authority or a replacement for product judgment.

## Repository

- Repository: [jpoindexter/product-management-skills](https://github.com/jpoindexter/product-management-skills)
- Primary language: not exposed by the accessible repository page
- License: MIT
- Stars: 1
- Forks: 0
- Open issues: not exposed by the accessible repository page
- Created date: not exposed by the accessible repository page
- Last pushed date: not exposed by the accessible repository page
- Main topics: `agent-skills`, `ai-agents`, `claude-code`, `codex`, `llm`, `product-discovery`, `product-management`, `product-strategy`
- Visible repository size: 2 commits, with `commands/`, `scripts/`, and `skills/` directories
- Releases: no release history was visible on the accessible repository page

## Why This Repo Was Picked

The winner is directly installable for Codex and Claude and has a narrow router that selects a small set of decision skills instead of dumping every framework into one answer. Its capability map covers discovery, interviews, opportunity trees, strategy, positioning, pricing, metrics, experiments, prioritization, roadmaps, PRDs, launches, stakeholder alignment, AI fit, AI evaluation, and AI risk. Each workflow is described with required inputs, decision steps, output contracts, quality gates, failure modes, and escalation rules, which gives a PO something to reuse in day-to-day work.

It also fills a gap in the vault. Existing notes cover larger PM skill libraries, planning templates, GitHub delivery automation, requirements standards, and product operating systems. This repo is a smaller Codex-native decision router with less setup and a clearer focus on choosing the right product decision workflow.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
| --- | --- | --- |
| [jpoindexter/product-management-skills](https://github.com/jpoindexter/product-management-skills) | Codex and Claude `/pm` router with decision skills for discovery, strategy, planning, metrics, experiments, launches, and AI product work | Won because the decision-oriented routing and explicit quality gates are practical despite weak community proof |
| [Uxcel-Lab/product-skills](https://github.com/Uxcel-Lab/product-skills) | 59 AI-agent skills, including 21 product-management skills, UX audits, product specs, roadmaps, metrics, experiments, and workflows | Strong documentation and MIT license, but the repo is also a broad UX toolkit and has more installation surface than this PO-focused shortlist winner |
| [julianoczkowski/product-manager](https://github.com/julianoczkowski/product-manager) | 18-stage Pragmatic Framework copilot that produces Markdown or Word artifacts from market problems through launch | More complete lifecycle dossier, but more opinionated, heavier, and tied to one framework and a longer guided journey |
| [tarunccet/pm-skills](https://github.com/tarunccet/pm-skills) | 93 skills, 63 commands, 9 plugins, MCP support, and workflows for discovery, strategy, execution, analytics, GTM, AI PM, and prototyping | Broad and useful, but the 100-plus-skill surface is harder to evaluate and the repository has only 7 stars |
| [Digidai/product-manager-skills](https://github.com/Digidai/product-manager-skills) | PM skills for SaaS metrics, PRD critique, roadmaps, discovery, and career coaching across Codex, Claude, Cursor, and Windsurf | Stronger visible adoption at 178 stars, but the CC BY-NC-SA 4.0 license limits commercial reuse and the scope is less clearly organized around a single PO operating loop |

## What It Is

This is a small skill library and command router, not a backlog application, project tracker, analytics product, or requirements database. The `skills/` directory contains reusable product decision procedures, `commands/` contains the `/pm` entry point and command definitions, and `scripts/validate.py` checks metadata, router targets, unresolved placeholders, and unwanted artifacts. The workflows produce decision-ready artifacts in the agent conversation; they do not write to Jira, Linear, GitHub Projects, or another system of record.

## Why It Is Useful For Product Owners

- Backlog refinement: use `product-prioritization` to choose a framework based on the decision context instead of applying RICE to everything.
- Discovery: use `product-discovery`, `product-interview`, and `product-opportunity-tree` to frame evidence gaps before committing to requirements.
- Requirements: use `product-prd` after the problem and evidence are clear, then inspect whether the output states measurable outcomes and unresolved assumptions.
- Stakeholder alignment: use `product-stakeholders` and `product-launch` to turn a decision into an owned communication and delivery plan.
- Roadmap planning: use `product-roadmap` to communicate outcomes and sequencing rather than presenting a fixed feature promise.
- Metrics and experimentation: use `product-metrics` and `product-experiment` to define success measures and tests before build work is treated as success.
- AI feature governance: use `product-ai-fit`, `product-ai-evals`, and `product-ai-risk` when the product decision involves model behavior, evaluation, or launch risk.

## How I Would Actually Use It

1. Run `/pm Which customer problem should we investigate next?` with interview notes, support themes, and usage evidence attached. Review the routed discovery output and keep the unanswered evidence questions visible.
2. Run `/pm Compare these three backlog opportunities` with strategic goals, customer impact, confidence, and effort. Use the resulting prioritization recommendation as a discussion aid, not an automatic ordering.
3. Run `/pm Turn this validated opportunity into a PRD` only after supplying the problem evidence, target user, constraints, and success measure. Reject any generated requirement that is not testable or traceable to the problem.
4. Run `/pm Turn this feature roadmap into an outcome roadmap` before a stakeholder review. Check that each theme has a strategy link, confidence level, and owner rather than only a date.
5. Run `/pm Design an experiment for the activation hypothesis` with the current baseline, target segment, primary metric, guardrails, and decision threshold. Put the proposed test into the team's normal experiment register.
6. Run `/pm Is this AI feature ready to launch?` with evaluation results, failure cases, user impact, and risk constraints. Use the output to create a launch checklist and explicit go or no-go decision.

## Limitations / Watch Outs

- One star and zero forks mean the workflows have almost no independent community validation.
- The repository has only two visible commits and no visible release history, so compatibility and maintenance are uncertain.
- The accessible GitHub page did not expose primary language, created date, last pushed date, or open-issue count. Do not treat missing metadata as evidence of health.
- Installation writes symlinks into both `~/.codex/skills/` and `~/.claude/skills/`; review `install.sh` before running it in a controlled environment.
- The router and skill wording can make a framework recommendation feel more rigorous than the underlying evidence. A PO still owns the decision and must challenge unsupported assumptions.
- There are no tracker, data warehouse, interview repository, or notification integrations. Inputs must be supplied manually and outputs must be copied into the team's real systems.
- The license covers the repository content, but the named books and frameworks remain the property of their authors and publishers. Check attribution and internal reuse requirements.

## Best Starting Points

- [README](https://github.com/jpoindexter/product-management-skills#readme): understand the router, capability map, installation, and validation command.
- [skills directory](https://github.com/jpoindexter/product-management-skills/tree/main/skills): inspect the individual decision workflows before installing anything.
- [commands directory](https://github.com/jpoindexter/product-management-skills/tree/main/commands): see how the `/pm` router maps requests to skills.
- [install.sh](https://github.com/jpoindexter/product-management-skills/blob/main/install.sh): review the symlink targets and installation behavior.
- [scripts/validate.py](https://github.com/jpoindexter/product-management-skills/blob/main/scripts/validate.py): see the repository's basic quality checks.
- [product-prioritization skill](https://github.com/jpoindexter/product-management-skills/tree/main/skills/product-prioritization): start with a concrete backlog decision.
- [product-experiment skill](https://github.com/jpoindexter/product-management-skills/tree/main/skills/product-experiment): start with a measurable learning decision.

## Metadata

- Scan date: 2026-10-26
- Canonical repository URL: https://github.com/jpoindexter/product-management-skills
- Duplicate detection: canonical GitHub repository URLs matching `github.com/<owner>/<repo>` were extracted from all Markdown files in the vault; this URL was absent before the note was created.
