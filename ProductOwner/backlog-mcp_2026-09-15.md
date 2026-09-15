---
title: backlog-mcp
date: 2026-09-15
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/corbym/backlog-mcp
repo: corbym/backlog-mcp
status: recommended
---

# backlog-mcp

## Verdict

This is worth a product owner's time if the team works in Git and wants an agent to operate on a real, reviewable backlog. It turns Markdown files into a small backlog system with epics, stories, statuses, acceptance criteria, notes, grooming, and pull-request updates. It is not a replacement for Jira or Linear, and its value depends on the team accepting repository-based workflow.

## Repository

- Repository: [corbym/backlog-mcp](https://github.com/corbym/backlog-mcp)
- Primary language: Go
- License: Unlicense
- Stars: 3
- Forks: 0
- Open issues: 0
- Created: 2026-04-13
- Last pushed: 2026-09-06
- Latest release: [v1.2.1](https://github.com/corbym/backlog-mcp/releases/tag/v1.2.1), published 2026-09-06
- Main topics: none listed

## Why This Repo Was Picked

It has a direct day-to-day PO use case rather than only advice or reading material. The repository stores a priority-ordered backlog, epics, stories, status, and acceptance criteria as ordinary Markdown under `requirements/`, so product decisions remain visible in Git history and reviewable by the team. Its MCP tools cover creation, refinement, status changes, notes, completion checks, and bulk updates, while the included GitHub Actions workflow connects story IDs to pull requests.

The shortlist favored practical workflow leverage, current maintenance, and low lock-in. `backlog-mcp` is small and lightly adopted, but it has a recent tagged release and a concrete operating model that a PO can trial in one project without migrating an entire organization.

## Shortlist Considered

| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [corbym/backlog-mcp](https://github.com/corbym/backlog-mcp) | MCP access to Git-backed epics, stories, statuses, acceptance criteria, notes, and PR automation | Won because it provides an executable backlog workflow with recent releases and low setup scope |
| [gabros20/product-skill](https://github.com/gabros20/product-skill) | Agent skill for discovery, strategy, PRDs, prioritization, metrics, and risks | Useful breadth, but it is an agent skill with 1 star, no open issues, and a last push in August; less immediately operational than a backlog system |
| [saurabh1chawda/product-discovery-toolkit](https://github.com/saurabh1chawda/product-discovery-toolkit) | Discovery frameworks, interview guides, canvases, experiments, and validation scorecards | Strong templates, but it was considered in the prior scan and overlaps with existing discovery coverage |
| [nmrtn/nanopm](https://github.com/nmrtn/nanopm) | Autonomous product-management workflow from discovery through delivery handoffs | Already covered in the vault and broader, heavier, and more agent-runtime dependent |
| [derrickgong87/product-idea-excavator](https://github.com/derrickgong87/product-idea-excavator) | Bilingual discovery interview and PRD skill | Good examples and MIT licensing, but it has no meaningful maintenance after April and is focused on idea-to-PRD work |

## What It Is

`backlog-mcp` is a local Model Context Protocol server written in Go. It is not a hosted project-management application. It reads and writes a repository-local `requirements/` directory containing an index, priority-ordered backlog, epic folders, and Markdown story files.

The server exposes structured operations for listing and reading stories, creating epics and stories, changing status, setting or checking acceptance criteria, adding notes, completing stories, grooming epics, and applying bulk updates. It also includes a GitHub Actions pattern that detects story IDs in pull requests and updates the matching backlog records.

## Why It Is Useful For Product Owners

- Backlog refinement: create stories with stable IDs, types, statuses, and acceptance criteria instead of leaving refinement decisions in chat.
- User stories: keep each story in a readable Markdown file that can be reviewed alongside the implementation.
- Acceptance criteria: replace criteria, check individual items, and block completion when criteria are missing or incomplete.
- Prioritization: maintain a numbered `backlog.md` file as the explicit order of work.
- Delivery coordination: connect `STORY-NNN` IDs to branches and pull requests so delivery status feeds back into the backlog.
- Stakeholder alignment: use Git history and pull-request review to make scope, status changes, and completion notes auditable.
- Product operations: use index summaries, grooming, bulk updates, and epic status guards for regular backlog hygiene.

## How I Would Actually Use It

1. Start with one small product repository and run `backlog-mcp init` to create `requirements/`.
2. Turn a roadmap objective into an epic, then create a few `feature`, `bug`, `chore`, or `spike` stories with explicit acceptance criteria.
3. Ask an AI agent to list draft stories, read the full story content, and identify missing criteria before refinement.
4. Use `set_story_status` and timestamped notes during discovery or delivery reviews, committing the changes so the team has an audit trail.
5. Put the story ID in branch names and PR titles, then install the included workflow to update status and append PR notes automatically.
6. Run `groom_epic` before sprint planning to reconcile the epic summary, story files, and index data.
7. Use `complete_story` only after the criteria are set and checked, then use the completion summary as release evidence.

## Limitations / Watch Outs

- The community signal is weak: 3 stars, no forks, and no open issues do not prove long-term durability.
- It is not a visual board, roadmap presentation tool, reporting suite, or replacement for stakeholder-facing project management software.
- The team must be comfortable with Git, Markdown, MCP configuration, and merge conflict resolution.
- Local repository storage is excellent for auditability but awkward for non-technical stakeholders and cross-project portfolio views.
- The GitHub Actions workflow installs the latest Go binary during runs, so teams should pin versions if reproducibility matters.
- The Unlicense is permissive but provides no warranty; review the implications with the team's legal or security owner before standardizing it.
- The server currently targets agent workflows, so verify the MCP client behavior and permissions before allowing write access to a production backlog.

## Best Starting Points

- [README](https://github.com/corbym/backlog-mcp#readme)
- [Latest release v1.2.1](https://github.com/corbym/backlog-mcp/releases/tag/v1.2.1)
- [Example requirements directory](https://github.com/corbym/backlog-mcp/tree/main/requirements)
- [MCP tool implementation](https://github.com/corbym/backlog-mcp/blob/main/tools.go)
- [Backlog parser and file model](https://github.com/corbym/backlog-mcp/tree/main/parser)
- [GitHub Actions files](https://github.com/corbym/backlog-mcp/tree/main/.github)
- [Contribution guidance](https://github.com/corbym/backlog-mcp/blob/main/CONTRIBUTING.md)

## Metadata

- Scan date: 2026-09-15
- Canonical repository URL: https://github.com/corbym/backlog-mcp
- Duplicate detection uses the canonical GitHub repository URL, normalized to `https://github.com/<owner>/<repo>` and treated as the unique repository key.
