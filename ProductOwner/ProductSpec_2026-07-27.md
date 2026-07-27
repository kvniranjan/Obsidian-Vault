---
title: ProductSpec
date: 2026-07-27
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/gokulrajaram/ProductSpec
repo: gokulrajaram/ProductSpec
status: recommended
---

# ProductSpec

## Verdict
ProductSpec is worth a product owner's time if the team is using coding agents or wants tighter handoff discipline between product intent and delivery evidence. It is not a casual PM reading list. It gives you a structured spec format, parser, CLI, MCP server, examples, and agent skills for turning product intent into something an implementation workflow can validate.

## Repository
- Repository: [gokulrajaram/ProductSpec](https://github.com/gokulrajaram/ProductSpec)
- Owner/repo: `gokulrajaram/ProductSpec`
- Primary language: TypeScript
- License: MIT
- Stars: 195
- Forks: 26
- Open issues: 3
- Created: 2026-07-04T19:57:44Z
- Last pushed: 2026-07-19T03:24:03Z
- Latest release checked: [v0.23.0](https://github.com/gokulrajaram/ProductSpec/releases/tag/v0.23.0), published 2026-07-13
- Main topics: ai-agents, developer-tools, markdown, openspec, prd, product-management, productspec, spec-driven-development, speckit

## Why This Repo Was Picked
This won because it gives a PO a concrete operating artifact, not another advice library. The repo includes a product spec standard, examples, validation commands, MCP support, agent run receipts, decision traces, and docs for Codex, Cursor, and Claude Code. That maps directly to the ugly handoff problem: vague PRDs, drifting scope, unchecked acceptance criteria, and agents claiming done without evidence.

## Shortlist Considered
| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [gokulrajaram/ProductSpec](https://github.com/gokulrajaram/ProductSpec) | Product intent standard, parser, CLI, MCP server, examples, agent skills, evidence receipts, decision traces | Won because it connects PO intent, acceptance criteria, implementation evidence, and agent delivery control. |
| [asdecided/core](https://github.com/asdecided/core) | Requirements-as-code engine and read-only MCP server for repository decisions | Strong and practical, but more decision-retrieval infrastructure than PO-owned spec authoring workflow. |
| [king-of-the-grackles/reddit-research-mcp](https://github.com/king-of-the-grackles/reddit-research-mcp) | MCP server for Reddit-based customer discovery and competitive research | Useful for discovery, but narrower and dependent on Reddit signal quality. |
| [joeseesun/qiaomu-app-review-insights](https://github.com/joeseesun/qiaomu-app-review-insights) | App Store review analysis for pain points, opportunities, and version risk | Good voice-of-customer fit, but mobile-app specific and younger than the winner. |
| [makeplane/plane](https://github.com/makeplane/plane) | Open-source Jira, Linear, Monday, and ClickUp alternative | Strong PO delivery tool, but its canonical URL is already covered in the vault. |

## What It Is
ProductSpec is an open standard and toolchain for product intent. The repository contains the spec format, schema, parser package, CLI commands, MCP server, GitHub Action, examples, starter kit, agent skills, and documentation. It is best understood as a structured PRD and evidence harness for teams that want product intent to survive handoff into engineering and agent-led implementation.

## Why It Is Useful For Product Owners
ProductSpec helps a PO make acceptance criteria, scope boundaries, success metrics, AI evals, related evidence, and revision history explicit. That is directly useful for backlog refinement, requirements writing, stakeholder alignment, delivery coordination, launch review, and post-build learning. The strongest fit is a team where PRDs are handed to engineers or agents and the PO needs a stricter way to prove what was requested, what changed, and what evidence supports completion.

## How I Would Actually Use It
1. Convert one messy PRD into a Product Spec before sprint planning, then validate it with the CLI before engineering starts.
2. Add numbered acceptance criteria and success metrics so every story in the backlog points back to a stable product-intent item.
3. Use the agent handoff command before asking Codex or Cursor to implement a feature, then require evidence for each acceptance criterion before accepting the work.
4. Create an Agent Run receipt for AI-assisted implementation so the team can see which spec revision was used and whether scope drift occurred.
5. Use Decision Trace when stakeholder feedback or delivery constraints force a meaningful product change.
6. Keep examples from `examples/real-world/` as reusable patterns for specs covering platform, AI, support, checkout, and workflow features.
7. Add the GitHub Action later if the team wants CI to block invalid product specs.

## Limitations / Watch Outs
This is young software, created in July 2026, so adoption proof is still thin compared with mature PM platforms. It adds process overhead, and a PO who just needs a lightweight story template may find it too structured. The value is highest when the team already works in Git, uses coding agents, or cares about traceable acceptance criteria and evidence. It will not replace discovery, prioritization judgment, stakeholder negotiation, or product strategy.

## Best Starting Points
- [README](https://github.com/gokulrajaram/ProductSpec/blob/main/README.md)
- [SPEC.md](https://github.com/gokulrajaram/ProductSpec/blob/main/SPEC.md)
- [Get started with agents](https://github.com/gokulrajaram/ProductSpec/blob/main/docs/get-started-with-agents.md)
- [Use with Codex](https://github.com/gokulrajaram/ProductSpec/blob/main/docs/use-with-codex.md)
- [Agent handoff](https://github.com/gokulrajaram/ProductSpec/blob/main/docs/agent-handoff.md)
- [Evidence loop](https://github.com/gokulrajaram/ProductSpec/blob/main/docs/evidence-loop.md)
- [Repo maintenance](https://github.com/gokulrajaram/ProductSpec/blob/main/docs/repo-maintenance.md)
- [Examples](https://github.com/gokulrajaram/ProductSpec/tree/main/examples)
- [Starter kit](https://github.com/gokulrajaram/ProductSpec/tree/main/starter-kit)
- [Latest release](https://github.com/gokulrajaram/ProductSpec/releases/tag/v0.23.0)

## Metadata
Scan date: 2026-07-27. Canonical repository URL: https://github.com/gokulrajaram/ProductSpec. Duplicate detection uses the canonical GitHub repository URL, not filename or note title.
