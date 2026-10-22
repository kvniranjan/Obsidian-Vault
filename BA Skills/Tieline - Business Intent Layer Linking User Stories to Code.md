---
date: 2026-10-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-traceability, user-stories, acceptance-criteria, ai-assisted-ba, mcp, codebase-graph]
source: GitHub
---

# Tieline - Business Intent Layer Linking User Stories to Code

## What is it?
Tieline is an open-source "business intent layer" that sits alongside a codebase and keeps Capabilities, User Stories, and Acceptance Criteria (ACs) formally linked to the exact code and tests that implement them. Instead of requirements living in a separate document that drifts from reality, Tieline stores them as a reviewed YAML contract that is version-controlled with the code and graded against live evidence. It is built for teams where AI coding agents are shipping fast, so product intent needs to stay durable and traceable as the implementation changes underneath it.

## Why it matters for Business Analysts
BAs have long struggled with requirements traceability matrices going stale the moment developers refactor code. Tieline automates that link: a separate grading agent checks whether each Acceptance Criterion is still "supported," "partial," or "unsupported" by the current implementation, giving BAs a living, evidence-backed view of coverage rather than a point-in-time snapshot. Its "blast-radius" and dependency-tracing tools let a BA ask what a proposed change will actually touch before writing a change request, and because everything is reviewed through normal pull requests, BAs can participate in the same workflow developers use rather than a separate requirements tool. This is especially valuable in AI-assisted delivery, where agents can generate or modify code far faster than a BA can manually re-verify requirements coverage.

## How to use it in BA Workflows
1. **Requirements traceability at code-change speed** - Link each User Story and AC to the code/tests that satisfy it, and let the grader flag ACs whose evidence has changed after a refactor or an agent-driven commit.
2. **Impact analysis before approving changes** - Use `tieline code compile` and the dependency graph to run blast-radius analysis, showing a BA exactly which Capabilities and ACs a proposed code change could affect.
3. **Continuous requirements review via pull requests** - Fold requirements review into the existing PR process instead of a separate sign-off cycle, so Stories and ACs are reviewed alongside the implementation that satisfies them.
4. **Idea-to-production backlog tracking** - Use the "Observations" feature to track feature requests and bug reports from initial idea through to production, optionally syncing to Postgres for stakeholders without repo access.
5. **Governing AI coding agents' output** - Expose Tieline's MCP tools so an AI agent can look up the intent behind a file, trace which ACs its change affects, and avoid inventing unverified citations when reporting what it built.

## Key Features
- **Reviewed intent contract** - Stories and ACs are stored as YAML and change alongside the implementation, accepted through standard PR review.
- **Graded evidence** - A dedicated grading agent checks each changed AC against source evidence and labels it supported, partial, or unsupported.
- **Code topology compiler** - `tieline code compile` extracts symbols and static dependencies via Tree-sitter so agents and BAs can trace relationships and estimate change impact.
- **CI checks** - `tieline check` fails builds on invalid YAML, broken links, or stale generated artifacts, and flags ACs whose linked evidence has drifted.
- **MCP agent tools** - Lets AI agents query intent, acceptance criteria, and dependency/blast-radius data directly during development.

## Technology Stack
- **Languages:** TypeScript/Node.js
- **Dependencies:** Tree-sitter (source parsing), YAML (contract manifest), optional PostgreSQL (synced state), Model Context Protocol (agent tooling), GitHub Actions (CI)
- **License:** AGPL-3.0

## GitHub Resources
- [knoxgraeme/tieline](https://github.com/knoxgraeme/tieline) - The business intent layer for your codebase; grounds user stories and acceptance criteria in the code that implements them.

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
