---
title: prd-template
date: 2026-11-12
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/SuperElectron/prd-template
repo: SuperElectron/prd-template
status: recommended
---

# prd-template

## Verdict

This is worth a product owner's time if the team is willing to keep product decisions in Git. It gives you usable PRD, decision, research, and JTBD artifacts plus a review process that makes assumptions, metrics, scope, and trade-offs visible. The repository has almost no adoption proof and its best workflow depends on Claude Code, so pilot it with one initiative instead of treating it as a mature product operating system.

## Repository

- Repository: [SuperElectron/prd-template](https://github.com/SuperElectron/prd-template)
- Primary language: Shell
- License: MIT
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-03-25
- Last pushed: 2026-08-26
- Main topics: none listed
- Releases: none listed

## Why This Repo Was Picked

The winner is practical because the templates are the product, not just prompts describing how a PO should work. The PRD template forces a problem statement, job stories, testable requirements, primary and guardrail metrics, anti-goals, constraints, risks, and review decisions. The surrounding workflow adds decision records, cited research briefs, JTBD analysis, PR review, naming rules, Markdown checks, secret protection, and GitHub pull requests, while the standalone templates still work without Claude Code or paid services.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [SuperElectron/prd-template](https://github.com/SuperElectron/prd-template) | PRD, decision, research, and JTBD templates with Claude skills and GitHub review workflow | Won because a PO can copy the templates immediately and use the review gates without installing the AI layer |
| [MJLeach87/AI-PM-OS](https://github.com/MJLeach87/AI-PM-OS) | Broad AI-augmented PM operating system with identity, execution, metrics, templates, MCP, and validation | More ambitious and more setup-heavy; the repository is better suited to a team willing to adopt a full operating system |
| [dasmeta/development-orchestrator](https://github.com/dasmeta/development-orchestrator) | Cross-repository orchestration for intent, contracts, implementation, validation, and delivery stages | Useful for multi-repo engineering organizations, but too infrastructure-heavy for ordinary PO backlog and discovery work |
| [Nelliesohl/agile-development-template](https://github.com/Nelliesohl/agile-development-template) | GitHub Projects templates for user stories, backlog, prioritization, estimates, iterations, and Kanban | Directly relevant, but maintenance is stale since 2024-12-28 and the workflow is narrower and less documented |
| [mirichard/pm-tools-templates](https://github.com/mirichard/pm-tools-templates) | Large library of project, program, product, stakeholder, risk, and planning templates | Stronger community proof, but already covered in the vault and much broader, which adds selection overhead for this focused use case |

## What It Is

This is a GitHub template repository for a Markdown-first product documentation workspace. It contains standalone templates and examples for PRDs, decision records, and research briefs, plus Claude Code commands and skills for authoring, JTBD analysis, research, review, workflow, and setup. It is not a backlog application, roadmap database, analytics tool, or system of record. GitHub pull requests, branches, labels, and CI provide the collaboration and quality-control layer.

## Why It Is Useful For Product Owners

- Backlog refinement: turn a vague request into a problem, job story, functional requirement, acceptance-ready scope, and explicit out-of-scope list.
- User stories and acceptance criteria: use the PRD structure to connect user jobs to requirements and measurable completion conditions.
- Prioritization: make opportunity, timing, guardrails, constraints, and trade-offs visible before ranking an initiative.
- Discovery: capture research questions, findings, sources, recommendations, and open questions in a reusable brief.
- Stakeholder alignment: use decision records to document alternatives, the chosen path, benefits, and trade-offs in one reviewable place.
- Roadmap planning: keep initiatives as dated, status-labeled artifacts with scope boundaries and links to the planning system rather than hiding the rationale in meetings.
- Metrics and experimentation: define a primary metric and counter metric in the PRD, then record the evidence and recommendation in a research brief after launch.
- Delivery coordination: use pull requests, review history, issue links, and CI checks to make product decisions visible to design and engineering.

## How I Would Actually Use It

1. Copy `docs/templates/prd-template.md` into `prds/2026-11-12_notification-preferences.md`, replace the placeholders, and require a baseline, target, timeframe, guardrail, anti-goal, and named dependency before requesting review.
2. Start a decision record for a build-versus-buy choice and require at least two credible alternatives with a specific rejection reason for each.
3. Put interview notes, support themes, and competitor findings into `research/`, then link the brief from the related PRD instead of pasting untraceable conclusions into a planning ticket.
4. Run the JTBD analysis on a proposed feature to test whether the job story describes a real situation and desired outcome rather than a disguised solution.
5. Open a pull request for each material product decision, ask design and engineering to review the scope and risks, and keep the review table in the PRD as the decision log.
6. Use the PRD review checklist before sprint planning to catch missing metrics, dependencies, risks, out-of-scope boundaries, or a status that is still marked Draft.

## Limitations / Watch Outs

- Adoption proof is weak: the repository has 0 stars, 0 forks, no listed topics, and no release history.
- The latest push was 2026-08-26, so the project is not demonstrating active maintenance at scan time.
- Claude Code is the recommended workflow and the setup path can involve GitHub, web search, and optional business-system connectors. The plain templates work without it, but the AI-assisted experience is not runtime-neutral.
- Git and Markdown are poor substitutes for a backlog, roadmap, or stakeholder notification system. You still need Jira, Linear, GitHub Projects, or another system of record for execution state.
- The templates encourage good questions but do not validate the truth of metrics, customer evidence, estimates, or prioritization claims. A polished PRD can still encode a bad decision.
- Optional integrations can expose customer or company data to external tools. Use least-privilege credentials and follow your organization's data-handling rules.
- The sample PRD includes illustrative metrics and links. Treat examples as format guidance, not evidence to reuse.

## Best Starting Points

- [README](https://github.com/SuperElectron/prd-template/blob/main/README.md)
- [Setup guide](https://github.com/SuperElectron/prd-template/blob/main/docs/guide.md)
- [PRD template](https://github.com/SuperElectron/prd-template/blob/main/docs/templates/prd-template.md)
- [Decision template](https://github.com/SuperElectron/prd-template/blob/main/docs/templates/decision-template.md)
- [Research template](https://github.com/SuperElectron/prd-template/blob/main/docs/templates/research-template.md)
- [PRD example](https://github.com/SuperElectron/prd-template/blob/main/docs/examples/prd-example.md)
- [PRD review checklist](https://github.com/SuperElectron/prd-template/blob/main/.claude/skills/prd-review/SKILL.md)
- [Workflow skill](https://github.com/SuperElectron/prd-template/blob/main/.claude/skills/prd-workflow/SKILL.md)

## Metadata

- Scan date: 2026-11-12
- Canonical repository URL: https://github.com/SuperElectron/prd-template
- Duplicate detection uses the canonical GitHub repository URL, normalized by owner and repository name, across every visible Markdown file in the vault.
