---
title: pm-handbook
date: 2026-09-04
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/brandonwise/pm-handbook
repo: brandonwise/pm-handbook
status: recommended
---

# pm-handbook

## Verdict

Yes, this is worth a product owner's time if you want a small set of working assets instead of another theory dump. The useful parts are the CSV-to-ranked-backlog script, AI evaluation scorecard generator, decision checklist, and templates for PRDs, KPIs, launches, tradeoffs, stakeholders, and postmortems. It is not a mature product platform: community proof is effectively absent and the repository has been quiet since May 2026.

## Repository

- Repository: [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook)
- Primary language: Python
- License: README states MIT; GitHub did not report SPDX metadata and no LICENSE file was present in the repository tree
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-03-10
- Last pushed: 2026-05-21
- Main topics: none listed

## Why This Repo Was Picked

It won because it combines reusable product artifacts with small executable tools. A PO can turn a CSV into a scored backlog, apply confidence and strategic-fit gates, generate a launch decision scorecard with rollback triggers, and use playbooks that explicitly require measurable outcomes, out-of-scope boundaries, tradeoffs, and a do-nothing option. That is more actionable than another repository that only collects prompts or links.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook) | PM templates, playbooks, Python prioritization and AI evaluation tools | Won because it has runnable utilities plus practical artifacts and tests |
| [johnefemer/skillfish](https://github.com/johnefemer/skillfish) | Product-manager skill with prioritization, interviews, PRDs, and discovery | Promising, but smaller and less proven, with only 2 stars and 1 open issue |
| [tomershahar/pm-skills](https://github.com/tomershahar/pm-skills) | Skills and workflows for discovery, strategy, execution, and analytics | Broader but largely a skill collection; activity was limited to its initial March 2026 push |
| [growthbook/growthbook](https://github.com/growthbook/growthbook) | Feature flags, experimentation, and product analytics platform | Strong software, but already covered in the vault and carries a much higher setup burden |
| [dwyl/product-owner-guide](https://github.com/dwyl/product-owner-guide) | Practical guide to PO issues, stories, and acceptance criteria | Already covered in the vault and is guidance rather than a reusable toolkit |

## What It Is

This is a lightweight PM handbook repository, not a backlog SaaS product. It contains Markdown templates, short workflow playbooks, sanitized case-study examples, Python command-line tools, and pytest tests. The tools cover feature prioritization from CSV input, case-study generation, and AI workflow evaluation scorecards with offline, shadow, and launch stages.

## Why It Is Useful For Product Owners

- Backlog refinement: capture feature candidates in a consistent CSV and rank them by reach, impact, confidence, strategic fit, and effort.
- Prioritization: use a visible formula and hard confidence or strategic-fit thresholds instead of hiding judgment inside a roadmap.
- Discovery: follow the AI PM workflow to cluster raw user, support, and telemetry signals by recurring pain before discussing features.
- Requirements: start with the PRD template and enforce measurable outcomes plus explicit out-of-scope content.
- Stakeholder alignment: use the stakeholder update and tradeoff memo templates to make decisions and compromises legible.
- Metrics and experimentation: define a KPI tree and an AI evaluation scorecard with scenario owners, thresholds, severity, status, and rollback triggers.
- Delivery coordination: use the launch-readiness, postmortem, and weekly operating rhythm assets to keep decisions connected to execution evidence.

## How I Would Actually Use It

1. Export the current opportunity or feature list to CSV, score each item from 1 to 5, and run `tools/prioritize_features.py` before roadmap review.
2. Run the prioritizer twice, once with default weights and once with minimum confidence and strategic-fit thresholds, then bring excluded items to the decision meeting explicitly.
3. Copy `templates/prd-template.md` for a feature brief and refuse to send it to engineering until the measurable outcome and out-of-scope section are filled in.
4. For an AI feature, list real customer or support scenarios in the evaluation CSV, assign severity and owners, and use the generated scorecard to decide ship, hold, or pending.
5. Add rollback triggers to every launch-stage AI scenario and review them daily during a staged rollout.
6. Use `playbooks/decision-quality-checklist.md` as a five-minute pre-read check for a contentious prioritization or scope decision.
7. Convert a completed rollout into a sanitized case study so the team records outcomes rather than only preserving the original plan.

## Limitations / Watch Outs

- The repository has 0 stars, 0 forks, no releases, no topics, and no open issues. That is not evidence of broad adoption.
- Last push was 2026-05-21, so maintenance is uncertain and the toolkit may already be abandoned.
- GitHub did not expose license metadata and the tree had no LICENSE file; verify the author's MIT statement before redistributing it.
- The prioritization formula is a useful forcing function, not a validated decision model. Scores still depend on biased estimates and do not replace customer evidence.
- The AI scorecard generator is a planning and reporting aid. It does not run evaluations, validate thresholds, or supply production telemetry.
- Python and Git are required for the executable workflow, and the templates still need adaptation to a team's product vocabulary, tools, and governance.
- The scope favors technical PMs and AI products. A non-technical PO may get more value from the templates than from the scripts.

## Best Starting Points

- [README and quick start](https://github.com/brandonwise/pm-handbook#readme)
- [Prioritization scorecard template](https://github.com/brandonwise/pm-handbook/blob/main/templates/prioritization-scorecard-template.md)
- [AI evaluation scorecard template](https://github.com/brandonwise/pm-handbook/blob/main/templates/ai-eval-scorecard-template.md)
- [AI PM discovery workflow](https://github.com/brandonwise/pm-handbook/blob/main/playbooks/ai-pm-discovery-workflow.md)
- [Decision quality checklist](https://github.com/brandonwise/pm-handbook/blob/main/playbooks/decision-quality-checklist.md)
- [Prioritization tool](https://github.com/brandonwise/pm-handbook/blob/main/tools/prioritize_features.py)
- [Tests](https://github.com/brandonwise/pm-handbook/tree/main/tests)

## Metadata

- Scan date: 2026-09-04
- Canonical repository URL: https://github.com/brandonwise/pm-handbook
- Duplicate detection uses the canonical GitHub repository URL, normalized as `https://github.com/<owner>/<repo>` without a trailing slash.
