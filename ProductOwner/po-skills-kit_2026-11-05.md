---
title: po-skills-kit
date: 2026-11-05
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/rafauto/po-skills-kit
repo: rafauto/po-skills-kit
status: recommended
---

# po-skills-kit

## Verdict

Yes, this is worth a product owner's time if you use Claude and want repeatable backlog hygiene without buying another system. It combines prompt-driven PO workflows with deterministic checks for story quality, RICE scoring, and release-note grouping, which is more defensible than asking an LLM to judge its own output. It is also extremely new, with no adoption proof or release history, so treat it as a useful MVP to test rather than a trusted team standard.

## Repository

- Repository: [rafauto/po-skills-kit](https://github.com/rafauto/po-skills-kit)
- README: [README.md](https://github.com/rafauto/po-skills-kit/blob/main/README.md)
- Primary language: Python
- License: MIT
- Stars: 0
- Forks: 0
- Open issues: 2
- Created: 2026-11-05
- Last pushed: 2026-11-05
- Releases: none
- Main topics: `claude`, `llm`, `mcp`, `product-management`, `product-owner`, `python`, `streamlit`, `user-stories`

## Why This Repo Was Picked

It directly covers recurring PO work instead of offering only generic prompts: user-story drafting, backlog refinement, RICE prioritization, and release notes. The important design choice is that Claude writes and explains artifacts while tested Python code checks story rules, calculates scores, validates input, and groups commits. The repository also includes fictional examples, recorded eval fixtures, CI, an MCP interface, a CLI, and a no-account Streamlit demo, so a PO can try the workflow before wiring it into a team environment.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [rafauto/po-skills-kit](https://github.com/rafauto/po-skills-kit) | Claude skills, story linter, RICE calculator, backlog refinement, release notes, CLI, MCP, and demo app | Won because it puts deterministic checks behind common PO workflows and has a low-cost local trial path |
| [NaderAbsy/sprintwise](https://github.com/NaderAbsy/sprintwise) | Story readiness scoring, Jira import and sync, sprint scope-change tracking, and reports | Strong product, but it is a larger hosted application with no detected license metadata and more setup and account dependency |
| [willowdev-code/ado-lens](https://github.com/willowdev-code/ado-lens) | Azure DevOps MCP server with PO skills for work items, boards, sprints, wiki, tests, and delivery tracing | More operationally capable, but useful mainly to Azure DevOps and Claude users and heavier to install |
| [product-on-purpose/product-lifecycle-templates](https://github.com/product-on-purpose/product-lifecycle-templates) | Governed lifecycle bundles with templates, guides, examples, and quality gates | Already covered in the vault and broader than the immediate backlog-quality problem |
| [saurabh1chawda/product-discovery-toolkit](https://github.com/saurabh1chawda/product-discovery-toolkit) | Discovery frameworks, evidence scoring, templates, examples, and workshop artifacts | Already covered in the vault and focused upstream on discovery rather than recurring delivery mechanics |

## What It Is

This is a small Python package with three interfaces around the same core logic: a command-line tool, an MCP server, and a Streamlit demo. It also contains four Claude skill folders that guide conversation-level work: `write-user-story`, `refine-backlog`, `prioritize-rice`, and `release-notes`.

The code handles the parts that should be reproducible: Given/When/Then story checks, input validation, RICE calculation, tie-breaking, and Conventional Commit grouping. The LLM remains responsible for drafting, asking questions, and explaining results. It is a toolkit and workflow starter, not a backlog system, Jira replacement, analytics platform, or complete product operating model.

## Why It Is Useful For Product Owners

- Backlog refinement: identify duplicates, oversized items, missing acceptance criteria, unclear personas, dependencies, and stakeholder questions.
- User stories: turn raw requests into one story with explicit persona, benefit, happy path, edge case, and open questions.
- Acceptance criteria: check that scenarios have observable Given, When, and Then steps instead of trusting a prose review.
- Prioritization: calculate reproducible RICE scores, explain the top three, and flag rankings that are sensitive to Confidence.
- Stakeholder alignment: keep assumptions, questions, splits, and rationale visible in the generated artifacts.
- Delivery coordination: turn conventional commit input into customer, internal, or stakeholder release notes while hiding internal maintenance work.
- AI governance: treat pasted backlog content as data, use fictional examples, and keep deterministic checks outside the model's self-assessment.

## How I Would Actually Use It

1. Copy `skills/write-user-story` into a Claude skills directory and paste one stakeholder request at a time. Require the output to include open questions instead of allowing invented business rules.
2. Export a backlog to Markdown or CSV, run `po-kit lint` on story files, and use the errors as the agenda for the next refinement session.
3. Run `po-kit rice examples/backlog.csv` on a candidate list, then review the top three and any items whose position changes when Confidence moves from 80% to 50%.
4. Use the `refine-backlog` skill before sprint planning to classify each item as Ready, Clarify, Split, Merge, or Rewrite, while retaining the original title.
5. Connect the MCP server to Claude Desktop or Claude Code so the model can call `lint_story`, `score_rice`, and `build_release_notes` instead of reproducing formulas in prose.
6. Generate customer-facing release notes from `git log --oneline` after a release, then manually check that every line traces to a real commit and that internal work was not exposed.
7. Run the included offline tests and eval fixtures before changing the rules, so a local customization does not silently reduce story quality or alter the scoring contract.

## Limitations / Watch Outs

- The repository was created and pushed on 2026-11-05. Zero stars, zero forks, no releases, and only two open issues provide no meaningful adoption evidence yet.
- The Claude skills require Claude Code or Claude Desktop with skills enabled. The core CLI can run without an API key, but the conversational workflow is Claude-specific.
- RICE is only as good as Reach, Impact, Confidence, and Effort inputs. A reproducible score does not make weak estimates or strategic choices correct.
- The story linter checks form and observable language, not whether the problem matters, the proposed outcome is valuable, or the solution is viable.
- There is no Jira, Linear, Azure DevOps, GitHub Issues, product analytics, or system-of-record integration in the current MVP. The backlog still has to be copied or exported.
- The Streamlit demo uses fictional data and should not receive customer or personal information. Local execution reduces exposure, but team retention and access policies remain your responsibility.
- The roadmap lists missing capabilities such as WSJF, a configurable Definition of Ready, GitHub issue export, sprint goals, and PyPI publication. Do not assume those exist because the workflow sounds complete.

## Best Starting Points

- [README and quick start](https://github.com/rafauto/po-skills-kit/blob/main/README.md)
- [User-story skill](https://github.com/rafauto/po-skills-kit/blob/main/skills/write-user-story/SKILL.md)
- [Backlog-refinement skill](https://github.com/rafauto/po-skills-kit/blob/main/skills/refine-backlog/SKILL.md)
- [RICE skill](https://github.com/rafauto/po-skills-kit/blob/main/skills/prioritize-rice/SKILL.md)
- [Release-notes skill](https://github.com/rafauto/po-skills-kit/blob/main/skills/release-notes/SKILL.md)
- [Fictional examples](https://github.com/rafauto/po-skills-kit/tree/main/examples)
- [Offline evals and tests](https://github.com/rafauto/po-skills-kit/tree/main/tests)
- [Architecture decisions](https://github.com/rafauto/po-skills-kit/tree/main/docs/decisions)
- [Issues and roadmap](https://github.com/rafauto/po-skills-kit/issues)

## Metadata

- Scan date: 2026-11-05
- Canonical repository URL: https://github.com/rafauto/po-skills-kit
- Duplicate detection uses the canonical GitHub repository URL, normalized as `github.com/<owner>/<repo>`, across all Markdown files in the Obsidian vault.
