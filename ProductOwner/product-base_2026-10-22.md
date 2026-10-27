---
title: Product Base
date: 2026-10-22
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/davideme/product-base
repo: davideme/product-base
status: recommended
---

# Product Base

## Verdict

Product Base is worth a short pilot for a product owner who already works in Obsidian and wants a visible idea backlog without adopting Jira, Linear, or a hosted product tool. It turns Markdown notes into RICE-ranked, impact-versus-effort, and Now/Next/Later/Won't Do views. It is not proven enough to become a team system of record yet: the repository has one star, no topics, and depends on beta-style BRAT installs plus companion plugins.

## Repository

- Repository: [davideme/product-base](https://github.com/davideme/product-base)
- Owner/repo: `davideme/product-base`
- Primary language: TypeScript by source layout; GitHub's language summary was not exposed on the accessible page
- License: MIT
- Stars: 1
- Forks: 0
- Open issues: not exposed by the accessible repository page
- Created date: not exposed by the accessible repository page
- Last pushed date: not exposed by the accessible repository page; the page showed 31 commits and a current `main` branch
- Main topics: none listed

## Why This Repo Was Picked

This was the strongest new candidate because it is directly usable inside the existing Obsidian workflow rather than merely describing product practice. The repository supplies a structured idea-note template, calculated RICE fields, an impact-versus-effort view, and a drag-and-drop roadmap view while keeping the data as ordinary Markdown. That gives a PO an immediately testable prioritization surface with little migration risk, even though the project has weak community proof.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [davideme/product-base](https://github.com/davideme/product-base) | Obsidian idea notes, RICE scoring, impact-effort chart, roadmap board | Won because it is directly usable in this vault and has low data lock-in |
| [Dengk3Li/product-manager-skill](https://github.com/Dengk3Li/product-manager-skill) | Agent skills for product decisions, roadmaps, and requirements traceability | Useful but adds another agent-skill layer; less useful for persistent backlog visibility |
| [akhil08agrawal/product-management-skills](https://github.com/akhil08agrawal/product-management-skills) | 18 framework-driven skills for discovery, strategy, build, and growth | Broad and readable, but one commit and mainly prompt-oriented |
| [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook) | PM templates, prioritization scripts, AI evaluation workflows, and playbooks | Already covered in the vault; a refresh was not justified over this more Obsidian-specific gap |
| [saurabh1chawda/product-discovery-toolkit](https://github.com/saurabh1chawda/product-discovery-toolkit) | Discovery frameworks, interview guides, evidence ladders, and validation templates | Already covered and focused upstream on discovery rather than backlog and roadmap operation |

## What It Is

Product Base is an Obsidian community plugin, not a standalone product-management application or a template-only repository. It creates and maintains a `ProductBase` idea folder, a Markdown template, property validation configuration, and Obsidian Base views. The core view ranks ideas by RICE, an optional Scatter plugin plots impact against effort, and an optional Bases Kanban plugin provides a roadmap board.

## Why It Is Useful For Product Owners

- Backlog refinement: turn each candidate idea into a note with summary, problem, theme, impact, effort, confidence, and roadmap state.
- Prioritization: use the RICE score as a consistent starting point, then record why a PO overrode the numeric ranking.
- Roadmap planning: move ideas between Now, Next, Later, and Won't Do without copying them into another tracker.
- Stakeholder alignment: use the impact-effort view to make trade-offs visible during prioritization conversations.
- Discovery: keep evidence, links, assumptions, and open questions in the idea note before promoting work into a delivery artifact.
- Delivery coordination: use roadmap state and note links to connect an opportunity to PRDs, user stories, experiments, or release notes elsewhere in the vault.

## How I Would Actually Use It

1. Install Product Base through BRAT in a disposable copy of the vault and enable the built-in Obsidian Bases core plugin.
2. Create one idea note for every active opportunity, using the supplied fields instead of keeping a flat list in a meeting note.
3. Add a short evidence paragraph and source links to each idea before assigning Reach, Impact, Confidence, and Effort.
4. Review the RICE table weekly, challenge stale scores, and record the decision owner and next evidence needed in the note.
5. Use the impact-effort chart to separate quick wins from expensive bets during backlog refinement.
6. Use the roadmap board to communicate Now, Next, Later, and Won't Do decisions, then link promoted ideas to PRDs and acceptance criteria.

## Limitations / Watch Outs

- Community proof is weak: the repository shows 1 star, 0 forks, no listed topics, and no visible release history on the accessible page.
- It is not a complete PO workflow. It does not provide discovery interviews, user-story quality checks, stakeholder communications, delivery tracking, analytics, or experimentation management.
- Product Base is not yet in the Obsidian Community Plugins directory. Installation uses BRAT or a manual build.
- The full experience depends on three companion plugins that are also installed through BRAT: Scatter, Bases Kanban, and Propsec.
- Obsidian 1.9.10 or later is required for Bases support. Missing companions reduce functionality, and the plugin's beta dependencies can break after updates.
- RICE is a prioritization aid, not evidence. Do not let a precise-looking score replace customer evidence, strategy, capacity, or explicit trade-offs.
- The accessible GitHub page did not expose exact created, last-pushed, or open-issue counts, so those fields are recorded as unavailable rather than guessed.

## Best Starting Points

- [README](https://github.com/davideme/product-base#readme): overview, views, installation, customization, and minimum requirements
- [Idea template and generated views](https://github.com/davideme/product-base#overview): understand the note fields and RICE calculation
- [Companion plugin setup](https://github.com/davideme/product-base#required-plugins): check the BRAT dependencies before installing
- [Installation instructions](https://github.com/davideme/product-base#installation): use BRAT first; manual build is the fallback
- [Roadmap view](https://github.com/davideme/product-base#roadmap-view-kanban): see how roadmap movement writes back to frontmatter
- [Tests folder](https://github.com/davideme/product-base/tree/main/tests): inspect the project's available automated checks
- [Changelog](https://github.com/davideme/product-base/blob/main/CHANGELOG.md): check changes before upgrading a pilot

## Metadata

- Scan date: 2026-10-22
- Canonical repository URL: https://github.com/davideme/product-base
- Duplicate detection uses the canonical GitHub repository URL `https://github.com/<owner>/<repo>` as the unique key, regardless of filename or title.
