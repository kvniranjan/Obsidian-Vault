---
date: 2026-08-16
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, ai-assisted-ba, agentic-ai, mcp]
source: GitHub
---

# RTMX - AI-Native Requirements Traceability Matrix Tool

## What is it?
RTMX is a lightweight, Git-native CLI that manages a requirements traceability matrix as plain CSV files stored alongside code. Instead of requiring analysts to manually update completion status, it derives "what's built, what's tested, and what's next" directly from linked test results, and exposes that state to AI coding agents (Claude, Cursor, and others) over the Model Context Protocol.

## Why it matters for Business Analysts
Traceability matrices are core BA deliverables, but they rot the moment status tracking becomes a manual chore disconnected from actual delivery. RTMX closes that loop automatically, giving BAs and product owners a live, audit-ready view of requirement completion, dependencies, and critical path — sourced from git history rather than stale spreadsheets. As AI coding agents increasingly implement requirements directly, RTMX gives BAs a way to keep formally-written requirements as the governing source of truth for that agentic work, rather than having agents work off ad-hoc prompts with no traceability back to the signed-off spec.

## How to use it in BA Workflows
1. **Requirements-to-test traceability** - Author requirements as structured CSV rows with unique IDs and specifications, then link them to automated tests; `rtmx verify` confirms whether the delivered code actually satisfies the written requirement.
2. **Live status reporting** - Run `rtmx status` for a dashboard of completion across all requirements, replacing manual RTM spreadsheet updates and status meetings with a single command stakeholders can trust.
3. **Backlog and dependency grooming** - Use `rtmx backlog` and `rtmx next` to surface the highest-priority unblocked requirement and perform critical-path analysis across dependent requirements.
4. **Governing AI-assisted delivery** - Expose the requirement set to AI coding agents via `rtmx mcp-server` so agents pull the next requirement, implement and test against it, and mark it done only when verification passes — keeping agentic development traceable to BA-authored specs.
5. **Audit and change history** - Because requirements live as CSV in Git, every change to scope, priority, or specification is visible via `git blame` and diffs, giving BAs a built-in audit trail without a separate ALM tool.

## Key Features
- 33-command CLI covering status dashboards, backlog prioritization, dependency health checks, and orphaned-test detection (`rtmx health`)
- Automatic test-framework detection and verification across Go, Python/pytest, Rust, Node.js, Java, Elixir, Swift, Dart, Ruby, and more
- MCP server exposing 7 tools so AI agents can query and update requirement status directly
- No database or external service required — pure CSV + Git, portable and diffable
- Atomic claim/release mechanism for coordinating multiple agents working the same requirement set concurrently
- GPG-signed releases with a Software Bill of Materials for supply-chain assurance

## Technology Stack
- **Languages:** Go (single static, cross-platform binary; Linux, macOS, Windows on amd64/arm64)
- **Dependencies:** Cobra CLI framework, YAML parser (minimal, only 2 external dependencies)
- **License:** Apache 2.0

## GitHub Resources
- [rtmx-ai/rtmx](https://github.com/rtmx-ai/rtmx) - Git-native requirements traceability matrix CLI with MCP integration for AI coding agents

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
