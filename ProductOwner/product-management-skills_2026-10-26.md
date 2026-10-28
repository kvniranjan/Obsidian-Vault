---
title: product-skills
date: 2026-10-27
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/Uxcel-Lab/product-skills
repo: Uxcel-Lab/product-skills
status: recommended
---

# product-skills

## Verdict

This is worth a product owner's time if they use an AI assistant and want better judgment in the output, not just faster document generation. The 21 PM skills cover discovery, requirements, roadmaps, metrics, experimentation, prioritization, and audits, with two workflows that connect them. It is not a product system of record, and the last push was 2026-07-02, so treat it as a useful skill library with a maintenance question, not a dependable platform.

## Repository

| Field | Value |
|---|---|
| Repository | [Uxcel-Lab/product-skills](https://github.com/Uxcel-Lab/product-skills) |
| Owner/repo | `Uxcel-Lab/product-skills` |
| Primary language | Python |
| License | MIT |
| Stars | 36 |
| Forks | 8 |
| Open issues | 1 |
| Created | 2026-06-22 |
| Last pushed | 2026-07-02 |
| Topics | `ai-skills`, `claude-skills`, `design-skills`, `figma-skill`, `pm-skills`, `ux-skill` |
| Release | `v1.0.0`, published 2026-07-02 |

## Why This Repo Was Picked

It beat the other candidates because it has unusually strong coverage of the actual PO loop: frame the problem, discover evidence, write a spec, prioritize, define metrics, test assumptions, and audit the resulting artifacts. The PM folder is organized into 21 small `SKILL.md` files rather than one oversized handbook, and the `idea-to-plan` and `product-review` workflows make the collection usable without memorizing every skill name. It also supports copying one skill or installing through `npx skills`, which keeps setup and lock-in low.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [Uxcel-Lab/product-skills](https://github.com/Uxcel-Lab/product-skills) | 21 PM skills, two workflows, and five artifact and decision audits | Won: strongest balance of PO coverage, reusable judgment rules, low setup, and visible community proof |
| [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook) | Markdown templates, Python prioritization and AI evaluation tools, playbooks, and examples | Practical, but has zero stars or forks, no GitHub license metadata, and less discovery and stakeholder coverage |
| [guhcostan/product-superpowers](https://github.com/guhcostan/product-superpowers) | 18 composable skills covering discovery through launch, with agentic review and research helpers | Broad and promising, but Claude-first, created and pushed on one day, and has only 1 star |
| [product-on-purpose/pm-skills](https://github.com/product-on-purpose/pm-skills) | Large PM skill library with workflows, commands, and sample outputs | Stronger adoption, but already covered in the vault and overlaps with recent notes; no refresh was justified today |
| [mirichard/pm-tools-templates](https://github.com/mirichard/pm-tools-templates) | Role-based PM templates for backlogs, stories, stakeholders, roadmaps, and metrics | Useful reference material, but already covered and less executable than the selected skill library |

## What It Is

This is a curated toolkit of plain-text `SKILL.md` files for AI assistants. It is not a backlog application, analytics product, project tracker, or integration layer. The repository contains 38 UX skills and 21 PM skills, with the PM material split into foundations, deliverables, processes, audits, and workflows. Each skill gives an assistant decision rules, context gates, trade-offs, and output expectations for a specific product task.

## Why It Is Useful For Product Owners

- Backlog refinement: use the user-story skill to turn vague requests into who, what, and why statements, then use spec-quality or prioritization-rigor audits before planning.
- Discovery: use problem-statement, personas-jtbd, discovery, and assumption-testing to keep a stakeholder request from becoming an untested feature commitment.
- Acceptance criteria and requirements: use product-spec and user-story skills to expose scope, edge cases, assumptions, and measurable requirements before engineering handoff.
- Prioritization: use the prioritization process plus its audit to select a framework for the context, surface weak confidence, sequence work, and document what is explicitly not being done.
- Roadmap planning: use the roadmap skill to produce outcome-oriented Now-Next-Later communication instead of a false-precision date list.
- Metrics and experimentation: use okrs-kpis, analytics, experimentation-ab, and okr-metric-validity to define baselines, targets, guardrails, decision rules, and stop conditions.
- Stakeholder alignment and delivery: use product-review to inspect an existing artifact and return a single prioritized set of issues rather than separate uncoordinated critiques.

## How I Would Actually Use It

1. Copy `pm/foundations/problem-statement/SKILL.md` into the team's assistant skills directory and use it on the next stakeholder request before opening a feature ticket.
2. Run `pm/workflows/idea-to-plan/SKILL.md` on one candidate initiative, then compare its generated problem, discovery, prioritization, spec, and metrics sections with the team's current planning document.
3. Run `pm/audits/spec-quality/SKILL.md` against a draft PRD and require the author to close every high-severity gap before refinement.
4. Use `pm/processes/prioritization/SKILL.md` on a backlog slice, recording the strategy link, confidence, dependencies, and explicit parking-lot decisions instead of accepting a bare RICE ranking.
5. Use `pm/deliverables/roadmap/SKILL.md` to rewrite a feature list into outcome themes with confidence labels for the next stakeholder review.
6. Use `pm/processes/experimentation-ab/SKILL.md` to draft a hypothesis, sample-size approach, guardrails, and decision rule before approving an experiment.
7. Use `npx skills add Uxcel-Lab/product-skills --list` first, then install only the PM skills the team needs rather than adding the full UX and PM collection blindly.

## Limitations / Watch Outs

- The repository is an instruction layer, not a system of record. It will not update Jira, Linear, GitHub Projects, analytics, or a roadmap for you.
- Most value depends on the assistant receiving real customer evidence, strategy, constraints, and data. Without those inputs, polished output can still be invented.
- The last push was 2026-07-02, despite the repository being created only ten days earlier. Check for current compatibility and maintenance before standardizing on it.
- The source material is tied to Uxcel's learning library and links back to its commercial courses. That does not invalidate the skills, but it is a reason to review the provenance and keep internal standards explicit.
- The PM collection sits beside a much larger UX collection. A full install may add noise and increase prompt or maintenance surface area.
- The skill names and install commands may change. Verify the current index before scripting installation or referring to a skill in team documentation.
- Audits can create false confidence if treated as a quality gate without human judgment. They are checklists and reasoning prompts, not evidence that a product decision is correct.

## Best Starting Points

- [README](https://github.com/Uxcel-Lab/product-skills#readme)
- [Product management index](https://github.com/Uxcel-Lab/product-skills/blob/main/pm/README.md)
- [Idea to plan workflow](https://github.com/Uxcel-Lab/product-skills/blob/main/pm/workflows/idea-to-plan/SKILL.md)
- [Product review workflow](https://github.com/Uxcel-Lab/product-skills/blob/main/pm/workflows/product-review/SKILL.md)
- [Product spec skill](https://github.com/Uxcel-Lab/product-skills/blob/main/pm/deliverables/product-spec/SKILL.md)
- [Prioritization process](https://github.com/Uxcel-Lab/product-skills/blob/main/pm/processes/prioritization/SKILL.md)
- [PM skills directory](https://github.com/Uxcel-Lab/product-skills/tree/main/pm)
- [Release v1.0.0](https://github.com/Uxcel-Lab/product-skills/releases/tag/v1.0.0)

## Metadata

- Scan date: 2026-10-27
- Canonical repository URL: https://github.com/Uxcel-Lab/product-skills
- Duplicate detection uses the canonical GitHub repository URL, normalized to the `owner/repo` pair, across all Markdown files in the vault.
