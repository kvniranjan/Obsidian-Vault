---
date: 2026-11-19
type: skill
category: Business Analysis
tags: [business-analyst, skill, user-story-mapping, requirements-management, ai-assisted-ba-workflows, traceability]
source: GitHub
---

# Tiepoint - Living User Story and Acceptance Criteria Contract Grounded in Code

## What is it?
Tiepoint is an open-source tool that generates a living "business intent layer" — Capabilities, User Stories, and Acceptance Criteria — and links each one directly to the exact code and tests that implement it. A Tree-sitter-based code graph and an AI grading step keep that evidence honest, flagging links as `supported`, `partial`, or `unsupported` whenever the underlying code changes.

## Why it matters for Business Analysts
BAs routinely lose confidence that a written requirement still reflects what was actually built, especially once AI coding agents start making rapid changes. Tiepoint closes that gap by making User Stories and Acceptance Criteria first-class artifacts reviewed through normal pull requests, with automatic drift detection (`tiepoint check`) when code evolves without a matching requirement update. It also tracks "Observations" (feature requests, ideas, bug reports) through their lifecycle to production, giving BAs a structured way to manage intake without a separate backlog tool, and exposes requirement state to non-technical agents (product, research, support) via an optional database sync.

## How to use it in BA Workflows
1. **Requirements traceability** - Maintain a YAML contract of Capability → User Story → Acceptance Criteria → Scenario, each AC linked to its implementing code and tests as evidence, so BAs can prove coverage instead of asserting it.
2. **Drift detection in CI** - Run `tiepoint check` in a pipeline to fail builds when linked evidence goes stale, a contract becomes invalid, or generated review artifacts fall out of date — catching silent divergence between specs and delivered behavior.
3. **AI-assisted requirement drafting** - Invoke the Tiepoint skill inside a coding agent session so the agent proposes or updates Stories and ACs directly from the code it just wrote, which a BA then reviews in a generated `review.html` instead of writing specs from scratch.
4. **Impact analysis before approving a change** - Use `analyze_code_blast_radius` to see which accepted Acceptance Criteria a proposed code change may affect, helping a BA scope regression risk during change requests.
5. **Backlog and idea intake** - Capture incoming feature requests, bugs, and questions as append-only Observations, then shape them into planned User Stories without losing the original source context.

## Key Features
- Capability → User Story → Acceptance Criteria → Scenario contract stored as reviewable YAML beside the code
- Tree-sitter-derived code topology (symbols, dependencies, blast radius) kept separate from Git by default
- AI grader that checks each Acceptance Criteria's evidence against a closed, deterministic citation list
- MCP-style agent queries (e.g. "What implements this AC?", "Which criteria touch these paths?")
- Optional Postgres sync so non-technical agents can query accepted product state and manage Observations

## Technology Stack
- **Languages:** TypeScript (core), Tree-sitter parsers for multi-language code analysis (JavaScript, Python, Rust, SQL, and more)
- **Dependencies:** Node.js/npx CLI, optional PostgreSQL for cross-agent state sync
- **License:** AGPL-3.0

## GitHub Resources
- [knoxgraeme/tiepoint](https://github.com/knoxgraeme/tiepoint) - Living Story/AC contract and semantic graph grounded in code, tests, and organizational evidence

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
