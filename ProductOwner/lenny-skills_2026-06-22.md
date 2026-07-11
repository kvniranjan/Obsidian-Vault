---
title: lenny-skills
date: 2026-06-22
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/RefoundAI/lenny-skills
repo: RefoundAI/lenny-skills
status: recommended
---

# lenny-skills

## Verdict

This is worth a product owner's time if they already use Claude Code or another agent that can load Markdown skills. It turns product advice into 86 task-specific workflows for real work such as PRDs, feedback synthesis, roadmap prioritization, metrics, scoping, and stakeholder alignment. It is not a substitute for product judgment, and the lack of repository activity since January 2026 is a real maintenance warning.

## Repository

- **Repository:** [RefoundAI/lenny-skills](https://github.com/RefoundAI/lenny-skills)
- **Owner/repo:** `RefoundAI/lenny-skills`
- **Primary language:** Not reported by GitHub; the repository is primarily Markdown content
- **License:** MIT
- **Stars:** 1,075
- **Forks:** 136
- **Open issues:** 1
- **Created:** 2026-01-29
- **Last pushed:** 2026-01-31
- **Main topics:** `ai-agents`, `ai-assistant`, `claude`, `claude-code`, `llm`, `pm-tools`, `product-management`, `product-skills`, `skills`

Metadata was checked through the GitHub API on 2026-06-22. Counts will change.

## Why This Repo Was Picked

The repository won because it packages advice into reusable instructions instead of another reading list. The coverage maps unusually well to recurring PO work: writing PRDs, analyzing feedback, conducting user interviews, prioritizing a roadmap, defining success metrics, managing scope, running decision processes, and aligning stakeholders. Individual skills include a working sequence, principles, questions to ask, common mistakes, and deeper source notes, so a PO can use them during an active task rather than merely browse them.

The setup burden is modest for an AI-assisted workflow: install one skill or the full collection, then invoke it with project context. Its 1,075 stars and 136 forks show visible interest, but those numbers did not decide the result. The deciding factor was breadth of practical PO workflows with low per-task setup.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
| --- | --- | --- |
| [RefoundAI/lenny-skills](https://github.com/RefoundAI/lenny-skills) | 86 AI-agent skills for product, discovery, strategy, delivery, growth, and leadership work | Won because the workflows can be used directly across the PO job, with low incremental setup. |
| [dend/awesome-product-management](https://github.com/dend/awesome-product-management) | A large curated list of product management resources | Useful for learning, but it is primarily a reading index rather than an execution aid. |
| [vemetric/vemetric](https://github.com/vemetric/vemetric) | Self-hosted web and product analytics | Strong for metrics and behavioral analysis, but infrastructure and implementation effort make it a narrower PO recommendation. |
| [panphp/pan](https://github.com/panphp/pan) | Lightweight, privacy-focused product analytics for PHP applications | Practical only when the product uses PHP and engineering agrees to instrument it. |
| [wiredashio/wiredash-sdk](https://github.com/wiredashio/wiredash-sdk) | In-app feedback and analytics for Flutter products | Directly useful for feedback collection, but limited to Flutter and dependent on developer integration. |

## What It Is

This is a Markdown-based skill library for Claude Code and compatible AI agents. Each skill is a folder containing a `SKILL.md` instruction file and, where available, reference notes distilled from interviews on Lenny's Podcast. It is neither a backlog application nor a template-only repository. It is a prompt and workflow collection intended to make an agent follow a more structured approach to a specific product task.

The collection spans user research, strategy, planning, shipping, leadership, growth, go-to-market, AI products, and career work. PO-relevant examples include `analyzing-user-feedback`, `conducting-user-interviews`, `prioritizing-roadmap`, `problem-definition`, `scoping-cutting`, `setting-okrs-goals`, `stakeholder-alignment`, `writing-north-star-metrics`, and `writing-prds`.

## Why It Is Useful For Product Owners

- **Backlog refinement:** Use `problem-definition`, `prioritizing-roadmap`, and `scoping-cutting` to challenge weak items, compare trade-offs, and reduce oversized work.
- **User stories and acceptance criteria:** `writing-prds` and `writing-specs-designs` force clearer context, outcomes, scope boundaries, and unresolved decisions. They do not provide a complete acceptance-criteria method, so the PO still needs to add testable conditions.
- **Prioritization and roadmapping:** `prioritizing-roadmap`, `planning-under-uncertainty`, and `running-decision-processes` help expose confidence, constraints, competing bets, and the cost of saying yes.
- **Discovery:** `conducting-user-interviews`, `analyzing-user-feedback`, `designing-surveys`, and `usability-testing` support research planning and synthesis.
- **Stakeholder alignment:** `stakeholder-alignment`, `written-communication`, and `giving-presentations` help structure options, recommendations, objections, and communication sequencing.
- **Metrics and experimentation:** `writing-north-star-metrics`, `measuring-product-market-fit`, `retention-engagement`, `designing-growth-loops`, and `ai-evals` can improve measurement discussions and test design.
- **Delivery coordination:** `managing-timelines`, `shipping-products`, `post-mortems-retrospectives`, and `managing-tech-debt` provide prompts for execution risks and cross-functional trade-offs.

## How I Would Actually Use It

1. Install only `writing-prds`, then give the agent a problem statement, user evidence, business constraint, and delivery deadline. Ask it to identify missing context before drafting the PRD.
2. Feed a sanitized set of interview notes and support tickets to `analyzing-user-feedback`. Require a theme table with evidence count, affected user segment, impact, confidence, and recommended follow-up.
3. Use `prioritizing-roadmap` during quarterly planning. Provide the candidate initiatives, goals, capacity, dependencies, and confidence levels, then ask for explicit cuts and trade-offs instead of a ranked list with everything included.
4. Run `stakeholder-alignment` before an approval meeting. Supply each stakeholder's incentives and objections, then prepare three options, one recommendation, and a pre-alignment sequence.
5. Pair `writing-prds` with `scoping-cutting` before backlog refinement. Ask the agent to separate the smallest useful release from follow-on scope and list unresolved acceptance decisions.
6. Use `writing-north-star-metrics` with existing funnel data to challenge whether the chosen metric reflects delivered customer value, then define input metrics and guardrails for human review.
7. Use `post-mortems-retrospectives` after a missed release to separate planning errors, dependency failures, decision delays, and execution problems, with owners and due dates for each corrective action.

## Limitations / Watch Outs

- The last push was 2026-01-31, two days after repository creation. The repository gained visible usage, but ongoing maintenance is not proven.
- The skills compress advice from podcast interviews. Compression removes context, and expert opinions can conflict. Treat the output as prompts for judgment, not policy.
- Most skills are guidance and questions, not complete operational templates with required fields, scoring logic, or validation rules.
- The repository is designed around Claude Code. Other agents may need manual copying or format adjustments.
- Installing all 86 skills can create noise and inconsistent behavior. Start with three to five skills tied to current work.
- Product evidence may contain customer or company-sensitive information. Sanitize inputs and follow the organization's approved AI policy.
- AI-generated PRDs, research synthesis, priorities, and metrics still require source checks and accountable human decisions.

## Best Starting Points

- [README and installation instructions](https://github.com/RefoundAI/lenny-skills#readme)
- [All skills](https://github.com/RefoundAI/lenny-skills/tree/main/skills)
- [Writing PRDs](https://github.com/RefoundAI/lenny-skills/tree/main/skills/writing-prds)
- [Prioritizing roadmaps](https://github.com/RefoundAI/lenny-skills/tree/main/skills/prioritizing-roadmap)
- [Analyzing user feedback](https://github.com/RefoundAI/lenny-skills/tree/main/skills/analyzing-user-feedback)
- [Stakeholder alignment](https://github.com/RefoundAI/lenny-skills/tree/main/skills/stakeholder-alignment)
- [Initial release](https://github.com/RefoundAI/lenny-skills/releases/tag/v1.0.0)
- [Contribution guide](https://github.com/RefoundAI/lenny-skills/blob/main/CONTRIBUTING.md)

## Metadata

- **Scan date:** 2026-06-22
- **Canonical repository URL:** https://github.com/RefoundAI/lenny-skills
- **Duplicate detection:** Duplicate detection uses the canonical GitHub repository URL.
