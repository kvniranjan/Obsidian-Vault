---
title: pm-handbook
date: 2026-10-29
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

This is worth a product owner's time if you want lightweight operating assets you can copy into an existing workflow. It combines a CSV-to-ranked-backlog script, an AI ship or hold scorecard generator, and templates for PRDs, KPIs, launches, tradeoffs, stakeholders, and postmortems. It is not proven or actively maintained enough to adopt as a team standard without review.

## Repository

- Repository: [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook)
- Primary language: Python
- License: GitHub metadata does not detect a license; the README states MIT. Verify before redistribution.
- Stars: 0
- Forks: 0
- Open issues: 0
- Created: 2026-03-10
- Last pushed: 2026-05-21
- Main topics: none listed
- GitHub releases: none listed

## Why This Repo Was Picked

It won because the value is executable and bounded rather than merely inspirational. The prioritization workflow makes confidence and strategic fit explicit, supports custom weights and hard constraints, and writes a Markdown backlog. The AI evaluation workflow connects scenarios, thresholds, owners, severity, status, and rollback triggers to a launch decision. The templates and weekly rhythm then give a PO a usable operating loop around those outputs. It also adds little setup burden: Python and CSV are enough for the scripts, while the Markdown assets can be copied directly.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [brandonwise/pm-handbook](https://github.com/brandonwise/pm-handbook) | PM templates, weekly playbooks, prioritization and AI eval scripts | Won on immediate usability and low setup burden. |
| [julianoczkowski/product-manager](https://github.com/julianoczkowski/product-manager) | 17 Agent Skills covering market problems through launch | Broad and capable, but more framework-specific and agent-dependent than this scan needed. |
| [louis3979/pm-tech-skills](https://github.com/louis3979/pm-tech-skills) | 58 skills, 30 workflows, technical delivery rigor, and project memory | Strong coverage, but much heavier and Claude Code oriented; only 3 stars and last pushed 2026-09-21. |
| [mohammadrizvi624/pm-os](https://github.com/mohammadrizvi624/pm-os) | Seven plugin areas spanning discovery, strategy, execution, analytics, and marketing | Ambitious but last updated 2026-06-11 and requires a larger plugin and company-context setup. |
| [UitbreidenOS/UitKit](https://github.com/UitbreidenOS/UitKit) | Claude Code skills and agents for discovery, roadmaps, analytics, and delivery | Useful breadth, but it is a larger general AI toolkit with more noise and setup than the focused handbook. |

## What It Is

This is a small product-management template library with Python helper tools, tests, playbooks, and sanitized case-study scaffolding. It is not a backlog system, project tracker, or integration with Jira, Linear, GitHub Projects, or an analytics platform. Its center of gravity is the artifact layer: create a decision-ready document from structured inputs, then review it with the team.

## Why It Is Useful For Product Owners

- Backlog refinement: use the prioritization CSV to force each item to state reach, impact, confidence, strategic fit, and effort.
- Prioritization: change the weights for a specific strategy and apply confidence or strategic-fit thresholds to exclude weak roadmap candidates.
- Requirements: start with the PRD template and use the decision-quality checklist to expose vague or unsupported claims.
- Metrics: use the KPI tree template to connect a feature to measurable outcomes instead of output counts.
- Experimentation and AI quality: define offline, shadow, and launch scenarios with thresholds, owners, severity, actuals, and rollback triggers.
- Stakeholder alignment: turn the stakeholder-update template and weekly operating rhythm into a predictable communication cadence.
- Delivery learning: use the launch-readiness and postmortem templates to record evidence, risks, misses, and follow-up actions.

## How I Would Actually Use It

1. Export the current feature candidates to CSV, score them with the default formula, and inspect the top three against one measurable outcome before changing the roadmap.
2. Re-run the prioritizer with `--min-confidence 3.0` and `--min-strategic-fit 3.0` to make low-evidence requests visible as exclusions instead of quietly ranking them.
3. Copy the PRD and tradeoff memo templates into the team's working folder, then require a written do-nothing option for major bets.
4. Build an AI feature eval CSV with critical scenarios, thresholds, owners, failure modes, and rollback triggers before launch planning.
5. Run the eval generator after offline and shadow testing so the launch conversation starts from pass, fail, blocked, and pending evidence.
6. Use the weekly rhythm as a five-day checklist: outcome review, customer signal, spec cleanup, execution risk review, and stakeholder update.
7. After launch, use the postmortem and case-study scripts to preserve what happened, what changed, and what should be repeated.

## Limitations / Watch Outs

- Community proof is absent: the repository has 0 stars, 0 forks, and 0 open issues.
- Maintenance is stale for a current scan: the last push was 2026-05-21, with no listed release history.
- GitHub does not report a license, even though the README says MIT. Resolve that discrepancy before reusing the code commercially or redistributing it.
- The scoring formula is a prioritization aid, not evidence. Bad estimates or political inputs still produce precise-looking rankings.
- The scripts use CSV and local Markdown only. There is no system-of-record sync, permissions model, audit trail, or analytics connector.
- The AI eval workflow is useful only if the scenarios and thresholds come from real user, support, safety, and operational evidence.
- The handbook is aimed at technical and AI product work. A nontechnical PO may need to simplify the scorecards and add domain-specific governance.

## Best Starting Points

- [README](https://github.com/brandonwise/pm-handbook/blob/main/README.md)
- [Prioritization scorecard template](https://github.com/brandonwise/pm-handbook/blob/main/templates/prioritization-scorecard-template.md)
- [Prioritization script](https://github.com/brandonwise/pm-handbook/blob/main/tools/prioritize_features.py)
- [AI eval scorecard template](https://github.com/brandonwise/pm-handbook/blob/main/templates/ai-eval-scorecard-template.md)
- [AI eval generator](https://github.com/brandonwise/pm-handbook/blob/main/tools/generate_eval_scorecard.py)
- [Weekly operating rhythm](https://github.com/brandonwise/pm-handbook/blob/main/playbooks/weekly-operating-rhythm.md)
- [Tests](https://github.com/brandonwise/pm-handbook/tree/main/tests)

## Metadata

- Scan date: 2026-10-29
- Canonical repository URL: https://github.com/brandonwise/pm-handbook
- Duplicate detection uses the canonical GitHub repository URL, normalized to owner/repository, across all Markdown files in the vault.
