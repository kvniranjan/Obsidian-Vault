---
title: carls-product-os
date: 2026-07-31
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/carlvellotti/carls-product-os
repo: carlvellotti/carls-product-os
status: recommended
---

# carls-product-os

## Verdict
This is worth a product owner's time if they use AI agents or Markdown to run product work. It is not a product management app, and it will not replace Jira, Linear, Productboard, or Confluence. Its value is more practical: it gives a PO a copyable workspace structure, examples, templates, and workflows for keeping goals, tasks, research, PRDs, stakeholder updates, and quarterly planning in one agent-readable system.

## Repository
- Repository: [carlvellotti/carls-product-os](https://github.com/carlvellotti/carls-product-os)
- Owner/repo: `carlvellotti/carls-product-os`
- Primary language: Python
- License: Not declared in GitHub metadata and no API license object was available
- Stars: 221
- Forks: 62
- Open issues: 0
- Created date: 2026-02-05
- Last pushed date: 2026-03-27
- Main topics: None listed in GitHub metadata

## Why This Repo Was Picked
It won because it is a usable operating model, not another abstract PM reading list. The repo includes a blank workspace, a filled example workspace, PRD and project brief templates, weekly stakeholder update templates, quarterly planning workflows, user research synthesis workflows, active task queues, and agent skills for repeatable PM tasks. The adoption evidence is stronger than most new PO-agent repos in this scan, with 221 stars and 62 forks, even though the last push is not very recent.

## Shortlist Considered
| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [carlvellotti/carls-product-os](https://github.com/carlvellotti/carls-product-os) | Copyable PM workspace with blank and example operating systems, templates, workflows, task files, and agent skills | Won because it covers recurring PO work across goals, PRDs, discovery, planning, stakeholder updates, and task tracking |
| [CrashBytes/claude-product-owner](https://github.com/CrashBytes/claude-product-owner) | Claude Code plugin for user stories, acceptance criteria, backlog prioritization, and release planning | Directly PO-shaped, but much narrower and less mature than today's winner |
| [bha-ai-ui/AI-Agile-Story-Mentor](https://github.com/bha-ai-ui/AI-Agile-Story-Mentor) | One-purpose story mentor concept for INVEST stories and Gherkin acceptance criteria | Too thin: the repository is basically a one-line README at scan time |
| [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) | Large PM skills framework with Codex and agent guidance | Strong repo, but already covered in this vault |
| [publiccodenet/product-steering](https://github.com/publiccodenet/product-steering) | Template for feature requests, backlog, roadmap, and product steering | Already covered in a shortlist and stale since 2020 |

## What It Is
This is a personal product management operating system for Claude Code. Practically, it is a Markdown workspace template with two tracks: `BLANK-OS/` for copying into a real setup, and `EXAMPLE-OS/` showing how a PM might organize goals, tasks, meetings, projects, templates, research, workflows, and skills. It is a template and workflow repository, not a SaaS product, not a backlog database, and not a full product analytics platform.

## Why It Is Useful For Product Owners
For backlog refinement, it gives a visible `Tasks/active.md` pattern and enough structure to separate active work, queued work, waiting items, blockers, and next actions. For requirements work, the PRD template covers problem statement, evidence, user stories, success metrics, scope boundaries, launch plan, milestones, open questions, and technical risks. For discovery, the research summary template and user research synthesis workflow force participant counts, evidence strength, quotes, contradictions, recommendations, and decision linkage. For roadmap planning, the quarterly planning workflow links last-quarter review, input gathering, OKR drafting, leadership review, capacity checks, and roadmap communication. For stakeholder alignment, the weekly update workflow pushes status, metrics, blockers, risks, decisions needed, and asks into a repeatable Friday update.

## How I Would Actually Use It
1. Copy `BLANK-OS/` into a product workspace and fill out `GOALS.md` with owned product areas, metrics, stakeholders, and current-quarter goals.
2. Use `Tasks/active.md` as a PO control panel before sprint planning, with active work, queued work, waiting items, blockers, and next actions in one place.
3. Start a new initiative from `Templates/project-brief.md` before writing a full PRD, so the problem, evidence, strategic fit, scope, risks, and open questions are explicit early.
4. Draft a PRD from `Templates/prd.md` and keep the success metrics, guardrails, feature flags, rollout plan, and rollback plan in the same document as the user stories.
5. Run the user research synthesis workflow after interviews, especially the pattern extraction and quality checklist, before converting findings into roadmap changes.
6. Use the weekly stakeholder update workflow every Friday to produce a short status note with current metrics, blockers, next week priorities, decisions needed, and specific asks.
7. Use the quarterly planning workflow to turn company priorities, customer feedback, research, engineering capacity, and carryover work into measurable OKRs and a realistic roadmap.

## Limitations / Watch Outs
- It is heavily Claude Code oriented. A Codex, Copilot, Obsidian, Notion, or plain Git workflow can reuse the Markdown structure, but the agent behavior will need adaptation.
- It is a personal OS, not a team governance system. You still need agreed ownership, review rituals, access control, and a source of truth for delivery tickets.
- It does not integrate directly with Jira, Linear, Productboard, analytics tools, or customer feedback systems.
- The repo has no declared license in GitHub metadata, so reuse inside a company should be checked before copying wholesale.
- Last push was 2026-03-27. That is not dead, but it is not currently moving fast either.
- Some examples are intentionally fictional or course-oriented, so a PO should treat them as scaffolding, not as a finished product-process standard.

## Best Starting Points
- [README](https://github.com/carlvellotti/carls-product-os/blob/main/README.md)
- [BLANK-OS folder](https://github.com/carlvellotti/carls-product-os/tree/main/BLANK-OS)
- [EXAMPLE-OS folder](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS)
- [Example PRD template](https://github.com/carlvellotti/carls-product-os/blob/main/EXAMPLE-OS/Templates/prd.md)
- [Example project brief template](https://github.com/carlvellotti/carls-product-os/blob/main/EXAMPLE-OS/Templates/project-brief.md)
- [Example weekly update template](https://github.com/carlvellotti/carls-product-os/blob/main/EXAMPLE-OS/Templates/weekly-update.md)
- [Weekly stakeholder update workflow](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS/Workflows/weekly-stakeholder-update)
- [User research synthesis workflow](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS/Workflows/user-research-synthesis)
- [Quarterly planning workflow](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS/Workflows/quarterly-planning)
- [Draft PRD section skill](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS/.claude/skills/draft-prd-section)
- [Weekly update skill](https://github.com/carlvellotti/carls-product-os/tree/main/EXAMPLE-OS/.claude/skills/weekly-update)

## Metadata
- Scan date: 2026-07-31
- Canonical repository URL: https://github.com/carlvellotti/carls-product-os
- Duplicate detection uses the canonical GitHub repository URL, not the filename or note title.
