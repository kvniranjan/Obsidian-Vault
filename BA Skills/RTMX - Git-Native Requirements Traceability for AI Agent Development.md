---
date: 2026-08-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, ai-assisted-ba, requirements-tracing, agentic-ai]
source: GitHub
---

# RTMX - Git-Native Requirements Traceability for AI Agent Development

## What is it?
RTMX is a CLI tool that stores a requirements traceability matrix as plain CSV files inside a Git repository, then keeps it synchronized with reality by auto-verifying each requirement's status against actual test results. Instead of a spreadsheet or a heavyweight ALM tool, requirements, their dependencies, and their linked tests live next to the code, versioned and diffable like any other file. It ships as a single static Go binary with an MCP server mode, so AI coding agents (Claude Code, Cursor, and similar) can query and update the matrix directly.

## Why it matters for Business Analysts
BAs routinely lose the thread between a written requirement and what actually got built and tested — status updates go stale within days of a sprint starting. RTMX removes that manual bookkeeping: a requirement's state (todo, blocked, verified) is derived automatically from test execution rather than someone updating a ticket. As BA workflows increasingly involve directing AI coding agents rather than human developers, RTMX gives analysts a structured, machine-readable handoff format — the agent can be pointed at `rtmx next --one` to work the highest-priority unblocked requirement, and `rtmx verify` closes the loop by confirming the implementation actually satisfies the spec. The CSV-in-Git approach also means requirements review happens through normal pull request diffs, and `rtmx health` catches orphaned or circularly-dependent requirements before they cause downstream confusion.

## How to use it in BA Workflows
1. **Structured Requirements Authoring** - Write requirements as CSV rows (ID, specification text, priority, dependencies, linked test paths) instead of a Word document or wiki page, giving every requirement a stable, referenceable identifier from day one.
2. **AI Agent Handoff for Implementation** - Point an AI coding agent at the RTM via `rtmx mcp-server` or `rtmx next --one`; the agent implements against the specification and RTMX verifies completion automatically, letting the BA focus on defining intent rather than chasing status.
3. **Automated Status Reporting** - Run `rtmx status` for a live completion dashboard across requirements and phases, replacing manual "where do we stand" check-ins with a command that reflects actual test outcomes.
4. **Change Impact and Backlog Prioritization** - Use `rtmx backlog` for critical-path analysis when a stakeholder requests a change, and `rtmx health` to catch requirements that reference tests which no longer exist or that have circular blocking dependencies.
5. **Audit-Ready Traceability in Pull Requests** - Because the RTM is CSV in Git, every requirement change appears as a reviewable diff with full git-blame history, giving BAs and compliance reviewers a lightweight, always-current traceability record without exporting reports from a separate tool.

## Key Features
- **CSV-in-Git storage** — human-readable diffs, offline/air-gapped friendly, zero vendor lock-in
- **Automatic status derivation** — requirement completion is computed from test results, not manually updated
- **`rtmx next --one`** — surfaces the highest-priority unblocked requirement for an agent or developer to work next
- **`rtmx verify`** — runs the project's test suite and cross-references results against the RTM
- **`rtmx health`** — lints the matrix for orphaned tests, circular dependencies, and stale references
- **MCP server mode** — exposes read and mutation tools over JSON-RPC for direct AI agent integration
- **Broad test-framework auto-detection** — Go, Python/pytest, Rust/Cargo, Node.js/npm, Java/Gradle/Maven, Elixir/Mix, Swift, Dart, Ruby

## Technology Stack
- **Languages:** Go
- **Dependencies:** Minimal (Cobra CLI framework, YAML parser); single static binary, no runtime dependencies
- **License:** Apache License 2.0

## GitHub Resources
- [rtmx-ai/rtmx](https://github.com/rtmx-ai/rtmx) - Requirements traceability matrix package for closed-loop product development with agentic AI tools

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[rmToo - Git-Native Requirements Management Tool]]
