---
title: AI Discovery Toolkit
date: 2026-11-25
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/Phunkhouse/ai-discovery-toolkit
repo: Phunkhouse/ai-discovery-toolkit
status: recommended
---

# AI Discovery Toolkit

## Verdict

This is worth a product owner's time if discovery work currently lives in scattered chats, vague tickets, and unrecorded assumptions. It produces a structured brief with questions, options, scope, acceptance criteria, metrics, approvals, and an engineering handover, while explicitly allowing a no-build outcome. The recommendation is conditional: the repository was created and last pushed on 2026-11-24, has zero stars and forks, and has not been run under Codex according to its README.

## Repository

- Repository: [Phunkhouse/ai-discovery-toolkit](https://github.com/Phunkhouse/ai-discovery-toolkit)
- Primary language: Shell
- License: Not specified by GitHub repository metadata
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-11-24
- Last pushed: 2026-11-24
- Main topics: None listed
- Releases: None found

## Why This Repo Was Picked

It directly addresses the upstream PO failure mode of turning an untested request into a delivery commitment. The Rapid and Standard profiles separate facts, stakeholder statements, requirements, constraints, assumptions, questions, and conflicts; compare build and no-build options; define acceptance criteria and success metrics; and record approvals before handover. It is also unusually practical for an early repository: the output is ordinary Markdown in the target project, the installer supports Codex and Claude Code, and the repository includes worked examples, structural checks, behavioral scenarios, and a validation script.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [Phunkhouse/ai-discovery-toolkit](https://github.com/Phunkhouse/ai-discovery-toolkit) | Discovery skills for framing, assumptions, options, scope, metrics, stakeholder decisions, validation, and handover | Won because it covers the widest upstream discovery-to-delivery gap with low setup and explicit human approvals |
| [shmouses/scrumscribe](https://github.com/shmouses/scrumscribe) | Human-approved conversion of PO conversations into scoped Jira tickets | Useful but narrower and tied to Claude Code, Jira, and a v0.2 preview |
| [hamidalm/po-practice-lab](https://github.com/hamidalm/po-practice-lab) | Offline eCommerce PO simulator with lessons, practice tasks, and an AI prompt coach | Good for training, not a day-to-day discovery artifact or team workflow |
| [Fully-Powered-AI/product-management-workflow-templates](https://github.com/Fully-Powered-AI/product-management-workflow-templates) | Six plain-Markdown workflows for release notes, scope, roadmaps, pricing, and acceptance criteria | Lower setup, but less rigorous about evidence, decision rights, validation, and handover |
| [TilakMn/Plotline](https://github.com/TilakMn/Plotline) | Browser prototype for backlogs, boards, roadmaps, methods, and prioritization | Broader project-management surface, but only an early browser prototype with no shared workspace |

## What It Is

This is a portable AI skill and workflow repository, not a backlog application or a system of record. It contains three profiles: a 10 to 30 minute Rapid discovery, a multi-stakeholder Standard discovery, and a handover procedure. The skills create `docs/discovery/<slug>/brief.md` and, only after approval, `handover.md` in the project being investigated. The repository also includes templates, shared rules, examples, decision records, evaluation scenarios, shell validators, and an installer that links the skills into Claude Code or Codex directories.

## Why It Is Useful For Product Owners

- Backlog refinement: turn a feature request into a problem statement, explicit requirements, open questions, conflicts, and a bounded scope before writing tickets.
- User stories and acceptance criteria: convert approved scope into testable criteria without silently treating an assumption as a fact.
- Discovery: keep evidence types and sources visible, ask only questions that can change the decision, and record unresolved gaps.
- Prioritization: compare multiple options, including process change, existing tools, validation tests, and no-build outcomes, instead of ranking only feature ideas.
- Stakeholder alignment: map decision rights, prepare asynchronous question packs, and require explicit approvals for important decisions.
- Metrics and experimentation: define success measures and validation thresholds before testing, with unknown numbers labelled as unknown rather than invented.
- Delivery coordination: generate a concise, approved handover for engineering and detect when that handover becomes stale.

## How I Would Actually Use It

1. Give `discovery-rapid` a customer escalation or feature request and a 20-minute time budget. Use the resulting brief as the agenda for the next refinement session.
2. Run `discovery-standard` for a cross-team workflow change. Have Product, Support, Operations, and Engineering answer the generated decision questions asynchronously.
3. Use the facts, statements, assumptions, and conflicts register to mark which backlog details are evidence-backed and which still need research.
4. Force a comparison between building a feature, changing an operating process, running a manual pilot, and doing nothing before committing roadmap capacity.
5. Set a measurable validation threshold before a prototype or experiment, then record the result and decision in the brief instead of rewriting history afterward.
6. Ask the toolkit to hand over only the approved problem, scope, acceptance criteria, constraints, and metrics to engineering. Keep the discovery brief as the source of truth.
7. Reopen a stale handover when scope or evidence changes, rather than letting an old discovery decision silently drive implementation.

## Limitations / Watch Outs

- The repository is one day old at this scan, with no stars, forks, releases, or open issues. There is no meaningful independent adoption proof.
- The README says Codex compatibility is designed in but has not been run under Codex because no Codex CLI was available to the author. Test it on a real task before standardizing it.
- Claude Code or Codex is required to run the skills. The installer assumes a local clone and shell access, so this is not a zero-setup web tool.
- The structural checker validates form, IDs, approvals, placeholders, and stale handovers. It cannot judge whether the product insight, evidence, or recommendation is correct.
- The generated briefs are not a replacement for Jira, product analytics, research repositories, or stakeholder governance. They are an artifact layer that still needs a team operating model.
- The repository advises keeping confidential discovery out of public version control. Customer data, interview notes, and business-sensitive assumptions need deliberate access and retention controls.
- The toolkit's evidence discipline reduces fabrication risk but does not verify claims. A confident stakeholder statement can still be wrong.

## Best Starting Points

- [README and quickstart](https://github.com/Phunkhouse/ai-discovery-toolkit#readme)
- [Rapid discovery skill](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/skills/discovery-rapid)
- [Standard discovery skill](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/skills/discovery-standard)
- [Handover skill](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/skills/discovery-handover)
- [Worked examples](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/examples)
- [Behavioral evaluation scenarios](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/evals)
- [Validation scripts](https://github.com/Phunkhouse/ai-discovery-toolkit/tree/main/scripts)
- [Specification](https://github.com/Phunkhouse/ai-discovery-toolkit/blob/main/docs/SPEC.md)
- [Roadmap](https://github.com/Phunkhouse/ai-discovery-toolkit/blob/main/docs/roadmap.md)

## Metadata

- Scan date: 2026-11-25
- Canonical repository URL: https://github.com/Phunkhouse/ai-discovery-toolkit
- Duplicate detection uses the canonical GitHub repository URL, normalized for scheme, host, owner, repository name, optional `.git`, fragments, and trailing slash.
