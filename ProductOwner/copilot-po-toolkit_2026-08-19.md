---
title: copilot-po-toolkit
date: 2026-08-19
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/marking/copilot-po-toolkit
repo: marking/copilot-po-toolkit
status: recommended
---

# copilot-po-toolkit

## Verdict
This is worth a product owner's time if the team lives in Azure DevOps and already has GitHub Copilot available in VS Code. It is not a general PM operating system, and it has no community proof yet, but the prompt set maps directly to backlog hygiene, PBI drafting, feature decomposition, capacity checks, sprint review, and release communication.

## Repository
- Repository: [marking/copilot-po-toolkit](https://github.com/marking/copilot-po-toolkit)
- Owner/repo: `marking/copilot-po-toolkit`
- Primary language: PowerShell
- License: MIT
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-07-22
- Last pushed: 2026-08-18
- Main topics: none listed by GitHub
- Releases: no GitHub release object found at scan time

## Why This Repo Was Picked
It wins because it is built for actual PO workflow execution in Azure DevOps, not just reading or generic product advice. The repo includes a setup script, Copilot instructions, an ADO assistant agent, and prompt files for recurring product-owner tasks. The strongest point is that write operations are guarded: the agent is instructed to preview creates or updates and wait for explicit confirmation before saving.

## Shortlist Considered
| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [marking/copilot-po-toolkit](https://github.com/marking/copilot-po-toolkit) | Copilot prompts and an ADO assistant for backlog health, capacity, PBIs, features, release notes, sprint reviews, and standups | Won because it targets real Azure DevOps backlog work with setup and safety guardrails |
| [starspacegroup/apollo](https://github.com/starspacegroup/apollo) | Agile PO AI voice and text assistant with backlog features | More ambitious, but heavier setup and less clearly reusable for normal PO workflows |
| [ANcpLua/PRD-Template-Product-Requirements-Document](https://github.com/ANcpLua/PRD-Template-Product-Requirements-Document) | Browser-editable PRD template with Markdown export | Useful but narrow: mostly PRD authoring, not ongoing backlog or delivery work |
| [srmcguirt/product-management-ai-prompt-pack](https://github.com/srmcguirt/product-management-ai-prompt-pack) | Small prompt pack for PRDs, stories, sprint planning, and competitive analysis | Easy to copy, but too thin compared with a configured ADO workflow |
| [api-evangelist/product-backlog](https://github.com/api-evangelist/product-backlog) | Product backlog reference content and API-style metadata | More educational than operational for a working PO |

## What It Is
This is a GitHub Copilot prompt and agent configuration template for product owners and Scrum Masters who manage Azure DevOps backlogs. It contains `.github` Copilot instructions, an ADO assistant agent, prompt files, a VS Code MCP configuration for Azure DevOps, a PowerShell setup script, and SAFe 6 reference material. It is a workflow template, not a standalone backlog tool.

## Why It Is Useful For Product Owners
The value is in reducing the repetitive PO work around backlog cleanup and stakeholder-ready communication. The backlog-health prompt looks for missing acceptance criteria, missing estimates, unassigned current-sprint work, stale items, and orphaned PBIs. The write-PBI and write-feature prompts help turn rough intent into structured Azure DevOps work items with acceptance criteria, priority, estimates, value area, parent links, and optional release notes. The capacity, sprint-review, release-notes, standup-prep, decompose-feature, and refine-story prompts cover practical delivery coordination rather than abstract product strategy.

## How I Would Actually Use It
1. Run the setup script in a team-specific copy and replace the ADO org, project, team, domain context, and glossary placeholders.
2. Use `backlog-health` before refinement to identify PBIs missing acceptance criteria, estimates, owners, updates, or parent Feature links.
3. Use `write-pbi` during intake when a stakeholder gives a vague request, forcing the conversation into testable acceptance criteria and a clear value area.
4. Use `write-feature` for larger work and ask for WSJF only when prioritization is actually needed.
5. Use `decompose-feature` before sprint planning to split an oversized Feature into candidate PBIs.
6. Use `capacity-check` before committing to a sprint so overcommitment is visible before the team locks scope.
7. Use `sprint-review` and `release-notes` to turn completed work into stakeholder updates without manually digging through Azure DevOps.

## Limitations / Watch Outs
This only makes sense if the team uses Azure DevOps and Copilot Chat in VS Code. It depends on Azure DevOps MCP or extension tooling being configured correctly, so the first run is not zero-friction. The repo has no stars, no forks, no release object, and very limited community validation at scan time. The agent frontmatter names Claude Sonnet 4, so teams using GitHub Copilot models should treat that as a template detail to adapt, not a guaranteed runtime setup.

## Best Starting Points
- [README](https://github.com/marking/copilot-po-toolkit/blob/main/README.md)
- [Setup guide](https://github.com/marking/copilot-po-toolkit/blob/main/SETUP.md)
- [ADO assistant agent](https://github.com/marking/copilot-po-toolkit/blob/main/.github/agents/ado-assistant.agent.md)
- [Backlog health prompt](https://github.com/marking/copilot-po-toolkit/blob/main/.github/prompts/backlog-health.prompt.md)
- [Write PBI prompt](https://github.com/marking/copilot-po-toolkit/blob/main/.github/prompts/write-pbi.prompt.md)
- [Write Feature prompt](https://github.com/marking/copilot-po-toolkit/blob/main/.github/prompts/write-feature.prompt.md)
- [Azure DevOps MCP config](https://github.com/marking/copilot-po-toolkit/blob/main/.vscode/mcp.json)

## Metadata
- Scan date: 2026-08-19
- Canonical repository URL: https://github.com/marking/copilot-po-toolkit
- Duplicate detection uses the canonical GitHub repository URL.
