---
date: 2026-08-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-traceability, ai-assisted-ba, mcp, cli]
source: GitHub
---

# RTMX - AI-Native Requirements Traceability Matrix CLI

## What is it?
RTMX is a terminal-based tool that manages a requirements traceability matrix (RTM) as version-controlled CSV files inside a Git repository. Instead of manually updating tickets, requirement status is derived automatically from test results, and the tool exposes an MCP server so AI coding agents can query, prioritize, and verify requirements directly.

## Why it matters for Business Analysts
Traceability matrices are core BA deliverables, but keeping them in sync with delivery reality is a constant manual burden. RTMX closes that loop automatically: every requirement's status reflects whether its linked tests actually pass, giving BAs an always-current, auditable view of coverage without chasing developers for updates. Because the matrix lives as plain CSV in Git, BAs get human-readable diffs on every pull request and a full history of how requirements evolved — useful for audits, regulatory traceability, and stakeholder sign-off. Its MCP integration also makes it a practical bridge between BA specifications and AI-assisted delivery teams, letting agents build strictly against BA-authored intent rather than drifting from it.

## How to use it in BA Workflows
1. **Requirements-to-test traceability** - Define requirements as structured CSV rows, link each to its verifying tests, and let `rtmx verify` cross-reference test results against the matrix so status is always accurate.
2. **Progress reporting to stakeholders** - Run `rtmx status` to get completion metrics across all requirements for sprint reviews, steering committees, or audit checkpoints without building a manual report.
3. **Backlog prioritization with dependency awareness** - Use `rtmx backlog` and `rtmx next` to surface the highest-priority unblocked requirement, helping BAs sequence delivery around critical-path dependencies.
4. **Matrix quality assurance** - Run `rtmx health` before reviews to catch orphaned tests, circular dependencies, or gaps in coverage before they reach a compliance audit.
5. **AI-assisted delivery governance** - Expose the matrix via `rtmx mcp-server` so AI coding agents pull unblocked requirements, implement against the BA's specification, and get verified automatically — keeping AI-generated work traceable to signed-off requirements.

## Key Features
- Git-native CSV storage - requirements diff like code, with full version history and PR-reviewable changes
- Automatic status derivation - requirement completion is computed from real test results, not manually toggled
- Critical-path backlog analysis - `rtmx next`/`rtmx backlog` surface the highest-value unblocked work
- Matrix linting - `rtmx health` detects orphaned tests and circular dependencies
- Auto-detection of 10+ test frameworks (pytest, Jest, Cargo, Gradle, Maven, Mix, and more) with zero configuration
- Built-in MCP server exposing 7 tools for direct AI agent integration via JSON-RPC

## Technology Stack
- **Languages:** Go
- **Dependencies:** Cobra CLI framework, YAML parser (single static binary, minimal dependency footprint)
- **License:** Apache 2.0

## GitHub Resources
- [rtmx-ai/rtmx](https://github.com/rtmx-ai/rtmx) - AI-native requirements traceability matrix CLI with MCP server integration

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
