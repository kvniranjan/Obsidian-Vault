---
title: product-engineering
date: 2026-11-26
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/phuryn/product-engineering
repo: phuryn/product-engineering
status: recommended
---

# product-engineering

## Verdict

Yes, this is worth a product owner's time if the team uses Claude Code, Codex, Cursor, or similar coding agents. It gives the PO a usable operating loop from product proposal and assumptions through build review, release approval, and learning, instead of another collection of generic prompts. It is not a replacement for a backlog, analytics stack, or product strategy practice, and much of the value disappears if the team does not ship through coding agents.

## Repository

- Repository: [phuryn/product-engineering](https://github.com/phuryn/product-engineering)
- Primary language: Python
- License: MIT
- Stars: 818
- Forks: 99
- Open issues: 0
- Created: 2026-10-29
- Last pushed: 2026-11-26
- Main topics: agent-skills, ai-agents, claude-code, claude-code-marketplace, claude-code-plugins, claude-skills, codex, cursor, product-engineering, product-management
- Latest observed release: v1.24.1, published 2026-11-26

## Why This Repo Was Picked

It covers the product decisions that usually get lost when an agent starts coding: what problem is being solved, which assumptions matter, what acceptance evidence is needed, who reviews the work, and what must be true before release. The repository has six installable packs, tests, explicit skill boundaries, a full walkthrough, and author-reported case studies from three live products. It also supports Codex as well as Claude Code, which makes it more usable here than a Claude-only PM kit.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [phuryn/product-engineering](https://github.com/phuryn/product-engineering) | 38 installable skills for discovery, planning, build review, release, and operations | Won: strongest end-to-end PO workflow, active releases, MIT license, and substantial community proof |
| [G3root/feeblo](https://github.com/G3root/feeblo) | Self-hosted feedback boards, public roadmap, changelog, widget, API, and MCP | Useful product software, but AGPL, operationally heavy, and narrower than the day-to-day decision workflow needed for this scan |
| [ScrumGuides/ScrumGuide-ExpansionPack](https://github.com/ScrumGuides/ScrumGuide-ExpansionPack) | Maintained Scrum guidance and agent-assisted documentation | Strong framework reference, but it is less directly actionable for discovery, requirements, and release decisions |
| [shinpr/nautilus](https://github.com/shinpr/nautilus) | Repository-based hypotheses, prototypes, evidence, and PRDs | Good focused discovery workflow, but only 8 stars and no activity since 2026-10-22 |
| [levnikolaevich/claude-code-skills](https://github.com/levnikolaevich/claude-code-skills) | Broad Claude and Codex plugins for discovery, architecture, delivery, and QA | Serious alternative, but more engineering-control oriented and less concise for a PO adopting one workflow |

## What It Is

This is a collection of agent skills distributed as six installable packs, not a standalone product-management application. The skills are Markdown instructions plus supporting references, scripts, tests, plugin manifests, and examples. The main product pack covers proposing a direction, market and competitor research, value proposition, planning, UI decisions, and lifecycle work; companion packs cover agent teams, shipping, app stack, harnesses, and work humanization.

## Why It Is Useful For Product Owners

- Backlog refinement: turn an agreed change into scoped work with assumptions, phases, rough sizing, tests, and acceptance criteria.
- User stories and acceptance criteria: make the build plan name observable behavior and the evidence that proves it.
- Discovery: keep opportunities, alternatives, hypotheses, segments, value propositions, and open decisions in one reviewed proposal.
- Stakeholder alignment: present one proposal artifact with claims, sources, tradeoffs, and decisions instead of scattered chat output.
- Roadmap planning: connect a product idea to lifecycle stages, release gates, dependencies, and the earliest usable slice.
- Metrics and experimentation: use validation, product analytics, and uptime skills to define what must be measured and checked after release.
- Delivery coordination: separate coordinator, builder, and independent reviewer roles so the implementation agent does not certify its own work.

## How I Would Actually Use It

1. Install the `product` pack in a product repository and run `start-here` to identify whether the next useful step is discovery, proposal, planning, build, review, or release.
2. Ask `propose` to compare the requested feature with alternatives, including doing nothing, and produce one evidence-labeled proposal with open decisions.
3. Use the proposal to run a short stakeholder review: challenge the weakest assumption, choose the scope, and record the decision before asking an agent to build.
4. For a complex feature, ask for a lifecycle plan that includes phases, acceptance criteria, test strategy, dependencies, and the earliest point a user can try it.
5. Require a fresh `independent-review` pass after implementation and use the findings to refine the backlog rather than accepting the builder's own completion claim.
6. Before launch, use `release-gate` to check that what the product promises, what the code implements, and what the tests verify are aligned.

## Limitations / Watch Outs

- The workflow assumes a repository and a coding-agent operating model. It is a poor fit for a PO who needs a visual backlog, roadmap database, or stakeholder portal.
- Installation is not one universal command. Claude Code and Codex use different plugin paths, and the README warns that Codex installs are user-wide while Claude can use project scope.
- Several skills are SaaS and engineering flavored, with assumptions about screens, deployment, tests, hosting, and production operations that need pruning for non-software or non-SaaS work.
- The author reports three live products as evidence, but that is not independent validation of the skills' product judgment.
- 818 stars and frequent releases show attention, not outcome quality. There are no open issues, so the absence of an issue backlog is not proof that the workflow is mature.
- Agent output still depends on the evidence supplied, the quality of the repository, and human decisions. A rigorous template can make an unsupported product decision look well organized.
- The repository's scope overlaps with the separately maintained `phuryn/pm-skills` project. Installing both can create duplicate skills and confusing precedence.

## Best Starting Points

- [README and installation](https://github.com/phuryn/product-engineering/blob/main/README.md)
- [End-to-end walkthrough](https://github.com/phuryn/product-engineering/blob/main/WALKTHROUGH.md)
- [Author-reported case studies](https://github.com/phuryn/product-engineering/blob/main/CASE-STUDIES.md)
- [Product pack](https://github.com/phuryn/product-engineering/tree/main/product)
- [AI shipping pack](https://github.com/phuryn/product-engineering/tree/main/ai-shipping)
- [Agent harness pack](https://github.com/phuryn/product-engineering/tree/main/agent-harness)

## Metadata

- Scan date: 2026-11-26
- Canonical repository URL: https://github.com/phuryn/product-engineering
- Duplicate detection uses the canonical GitHub repository URL, normalized by owner and repository name, across all Markdown files in the Obsidian vault.
