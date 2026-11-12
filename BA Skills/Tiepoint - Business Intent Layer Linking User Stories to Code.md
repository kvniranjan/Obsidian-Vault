---
date: 2026-11-12
type: skill
category: Business Analysis
tags: [business-analyst, skill, user-story-mapping, requirements-traceability, ai-assisted-ba, github]
source: GitHub
---

# Tiepoint - Business Intent Layer Linking User Stories to Code

## What is it?
Tiepoint is an open-source tool that keeps product intent versioned alongside a codebase. It has AI agents generate Capabilities, User Stories, and Acceptance Criteria (ACs), then link each one to the specific code and tests that implement it, so the "why" behind a feature travels with the "how" through normal pull-request review.

## Why it matters for Business Analysts
Requirements drift from the code that implements them the moment documentation stops being updated alongside delivery — Tiepoint closes that gap by making Stories and ACs first-class, reviewable artifacts that change in the same pull request as the code. A grading agent checks whether changed ACs are actually `supported`, `partial`, or `unsupported` by source evidence, giving BAs a living, auditable trace between requirement and implementation instead of a stale BRD. Because intent is stored as YAML in the repo (with an optional Postgres sync), BAs, support teams, and other agents can query the accepted state of a feature without needing direct codebase access. This turns requirements traceability from a periodic manual exercise into a continuous, CI-enforced check.

## How to use it in BA Workflows
1. **Requirements traceability as code** - Capture Capabilities, User Stories, and Acceptance Criteria as versioned YAML tied to the commits and tests that satisfy them, replacing a separate traceability matrix maintained by hand.
2. **Evidence-graded acceptance criteria** - Use the grading agent's `supported` / `partial` / `unsupported` verdicts to spot ACs that were approved but never actually implemented, or that regressed after a later change.
3. **Backlog intake via Observations** - Log feature requests, ideas, and bug reports as Observations and track them through to production, giving BAs a lightweight funnel from stakeholder input to delivered behavior.
4. **CI-enforced requirements hygiene** - Run `tiepoint check` in CI to flag invalid YAML, broken links, and stale or changed evidence before a PR merges, so requirement documentation can't silently fall out of sync with code.
5. **Agent-queryable product knowledge** - Let support, research, or product agents query the accepted state of `main` through the optional Postgres sync, so "what does this feature actually do today?" has an authoritative, current answer.

## Key Features
- **Reviewed intent** - Stories and ACs change alongside code and are accepted through standard pull-request review, not a separate sign-off process.
- **Graded evidence** - A dedicated grading agent checks each changed AC against source evidence and returns a support verdict rather than trusting self-reported completion.
- **Code topology mapping** - `tiepoint code compile` records symbols and static dependencies via Tree-sitter so agents can trace which accepted behaviors a given code change might affect.
- **Observations pipeline** - Optional Postgres-backed tracking of feature requests, ideas, and bugs through to production.
- **CI checks** - `tiepoint check` catches invalid YAML, broken links, and stale or invented evidence citations automatically.
- **MCP tooling** - Exposes agent-facing tools so AI coding assistants can read and update product intent directly.

## Technology Stack
- **Languages:** TypeScript, Node.js
- **Dependencies:** Tree-sitter (parsing), optional PostgreSQL (shared state/sync), Docker, MCP tools, GitHub Actions (CI)
- **License:** AGPL-3.0

## GitHub Resources
- [knoxgraeme/tiepoint](https://github.com/knoxgraeme/tiepoint) - The business intent layer for your codebase; grounds user stories and acceptance criteria in the code that implements them.

## Related Skills
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
- [[Featmap - User Story Mapping]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
