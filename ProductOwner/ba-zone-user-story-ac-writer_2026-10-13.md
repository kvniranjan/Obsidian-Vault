---
title: ba-zone-user-story-ac-writer
date: 2026-10-13
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer
repo: phucnt-bazone-vietnam/ba-zone-user-story-ac-writer
status: recommended
---

# ba-zone-user-story-ac-writer

## Verdict

This is worth a product owner's time when stories reach refinement vague, oversized, or hard for QA to test. It gives a concrete INVEST and Given-When-Then workflow, templates, examples, split guidance, and a self-review checklist that can be copied into an existing team process. It is not a backlog tool, and its last code push was in May 2026, so use it as a practical writing aid rather than a maintained product platform.

## Repository

- Repository: [phucnt-bazone-vietnam/ba-zone-user-story-ac-writer](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer)
- Primary language: Not detected by GitHub; Markdown skill files
- License: MIT in `LICENSE`; GitHub API reports `NOASSERTION`
- Stars: 189
- Forks: 88
- Open issues: 0
- Created: 2026-05-09
- Last pushed: 2026-05-19
- Main topics: None listed

## Why This Repo Was Picked

It solves a narrow, repeated PO problem instead of adding another broad PM operating system. The repo enforces six INVEST checks, requires at least three acceptance-criteria scenarios, separates happy path, edge case, and negative path coverage, suggests story splits, and includes copyable templates plus seven worked examples. The setup is low: a PO can copy the Markdown into a project repository and adapt the domain examples without deploying software or changing the system of record.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
| --- | --- | --- |
| [phucnt-bazone-vietnam/ba-zone-user-story-ac-writer](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer) | User story and acceptance-criteria skill with INVEST, Gherkin, templates, examples, and a quality checklist | Won because it is immediately usable for refinement and QA handoff with minimal setup |
| [phucnt-bazone-vietnam/product-discovery](https://github.com/phucnt-bazone-vietnam/product-discovery) | BA elicitation skill focused on asking why and clarifying needs | Useful upstream, but less complete for the day-to-day story and acceptance-criteria handoff |
| [Elsevanderberg1/product-discovery-skills](https://github.com/Elsevanderberg1/product-discovery-skills) | Claude Code pipeline for ICP screening, opportunity mapping, clustering, sizing, and discovery | Strong discovery coverage, but requires transcript workflows and more setup than the selected artifact layer |
| [phuryn/pm-skills](https://github.com/phuryn/pm-skills) | Large PM skills marketplace covering discovery, strategy, execution, launch, and growth | Broad and actively maintained, but much heavier to evaluate and already covered in the vault |
| [aakashg/pm-planning-system](https://github.com/aakashg/pm-planning-system) | Version-controlled feature planning templates, review skill, rollout, and pilot measurement | Already covered in the vault and aimed at feature planning rather than story-level acceptance quality |

## What It Is

This is a Markdown-based Claude skill and template library, not a standalone application or backlog integration. `SKILL.md` defines three modes: write a new story, refine an existing story, or add acceptance criteria. The repository also contains an empty user-story template, a Given-When-Then acceptance-criteria template, INVEST reference material, seven domain examples, and a quality checklist. It is designed to be uploaded to a Claude Project or copied into a skills directory, but the underlying Markdown can be adapted to other assistants or a manual team workflow.

## Why It Is Useful For Product Owners

- Backlog refinement: turn a feature description into a bounded story with a specific persona, goal, business value, dependencies, assumptions, and estimate metadata.
- User stories: prevent generic personas, vague goals, duplicated value statements, and stories that bundle several CRUD operations or personas.
- Acceptance criteria: require at least one happy path, one edge or validation case, and one negative path in Given-When-Then form.
- Delivery coordination: make the story small enough to estimate and expose dependencies, assumptions, and open questions before sprint commitment.
- QA collaboration: give QA testable outcomes without dictating API names, database schema, or pixel-level UI implementation.
- Prioritization: retain priority and epic fields in the template, while keeping the actual priority decision with the product team.
- Stakeholder alignment: use the INVEST table and explicit business value to expose disagreement before development starts.

## How I Would Actually Use It

1. Copy `templates/user-story-template.md` and `templates/ac-template.md` into the product repository or adapt them to the team's Jira, Linear, or Azure DevOps format.
2. Pick one story that repeatedly returns from refinement and run it through the three checks: specific persona, measurable goal, and distinct business outcome.
3. Use the INVEST table to mark failures, then split stories with multiple personas, CRUD operations, business rules, or more than 7 to 8 scenarios.
4. Write three minimum acceptance-criteria scenarios for the next story: happy path, boundary or race condition, and permission, validation, or error path.
5. Replace the EdTech examples in `references/examples.md` with examples from the team's domain so the generated wording uses real roles, states, and business rules.
6. Run the quality checklist with a developer and QA partner before sprint planning, recording unresolved dependencies and open questions instead of hiding them in a meeting.
7. Compare the resulting story against the team's existing Definition of Ready and keep only the checks that reduce clarification churn.

## Limitations / Watch Outs

- The repository is Claude-oriented. `SKILL.md` and the installation steps need adaptation for Codex, Copilot, a manual process, or a different agent runtime.
- The README and examples are primarily Vietnamese and EdTech-flavored. The content is usable, but the examples should be translated or replaced for another domain.
- GitHub reports no detected language and `NOASSERTION` license metadata, although the checked-in `LICENSE` says MIT and adds an attribution requirement. Confirm the terms before redistribution.
- The last push was 2026-05-19, with only two visible commits and no GitHub release. The repository may be intentionally complete, but there is little maintenance evidence.
- INVEST is a useful conversation tool, not proof that a story is valuable or that the underlying discovery is sound.
- The checklist cannot validate business rules, accessibility, legal constraints, analytics instrumentation, or architecture. Human product, engineering, design, and QA review remains necessary.
- Copying every rule into a rigid Definition of Ready can create ceremony. Pilot it on a small set of stories and measure rework or clarification rounds.

## Best Starting Points

- [README](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer#readme)
- [SKILL.md](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/SKILL.md)
- [User story template](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/templates/user-story-template.md)
- [Acceptance criteria template](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/templates/ac-template.md)
- [Quality checklist](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/checklists/quality-checklist.md)
- [INVEST reference](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/references/invest-criteria.md)
- [Worked examples](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/references/examples.md)
- [License](https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer/blob/main/LICENSE)

## Metadata

- Scan date: 2026-10-13
- Canonical repository URL: https://github.com/phucnt-bazone-vietnam/ba-zone-user-story-ac-writer
- Duplicate detection uses the canonical GitHub repository URL `https://github.com/<owner>/<repo>` as the unique key across Markdown files.
