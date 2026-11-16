---
date: 2026-11-16
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, business-rules, decision-table, scorecard, python, ai-assisted-ba]
source: GitHub
---

# Decikit - Python Decision Pipeline and Business Rules Toolkit

## What is it?
Decikit (the "decider toolkit") is an open-source Python package, maintained by Capitec Bank's Data Science Platform team, for building decision pipelines out of decision trees, decision tables, and scorecards. Instead of hand-coding a rules engine, a BA or developer can express decision logic as plain Python functions or as JSON-configured steps, which the toolkit then runs over single records or whole polars DataFrames. It is purpose-built for high-volume, auditable decisioning such as credit, affordability, or eligibility checks.

## Why it matters for Business Analysts
Decision management is a core BA discipline, and Decikit gives BAs a lightweight, inspectable way to document and operationalize business rules without needing a full DMN engine stack. Decision tables and scorecards can be authored and versioned as plain JSON, making them readable and reviewable by non-developers in the same way a BA would review a decision table in a requirements doc. Runtime-tunable parameters mean thresholds (e.g., a debt-to-income limit) can be adjusted by business stakeholders without a code change or redeploy. It also directly supports AI-assisted BA workflows: it ships a Claude Code plugin with a skill and MCP server specifically for reading, editing, and validating decision pipelines, trees, tables, and scorecards.

## How to use it in BA Workflows
1. **Document business rules as decision tables** - Capture eligibility, pricing, or approval logic as JSON-configured decision tables that map directly to how BAs typically document rules in a requirements or decision-model artifact.
2. **Model scorecards for risk/eligibility decisions** - Use the built-in scorecard step type to represent weighted scoring logic (e.g., credit risk scoring) in a transparent, auditable format business stakeholders can review.
3. **Tune thresholds without engineering cycles** - Expose business-owned parameters (limits, cutoffs, weights) via `param()` so BAs and business owners can adjust decision thresholds per environment or run without a code change.
4. **Prototype and validate decision logic with AI assistance** - Use the included Claude Code plugin/MCP server to have an AI agent read, edit, and validate decision trees/tables/scorecards, speeding up collaborative rule authoring between BAs and engineers.
5. **Serve decisions for stakeholder demos or integration testing** - Stand up the pipeline as an HTTP service (via uvicorn/starlette or sanic) so BAs can validate rule outcomes against real or sample data during UAT.

## Key Features
- **Composable pipelines** - Steps combine via `flow`, `dag`, `branch`, and `loop` primitives to model sequential, parallel, conditional, or iterative decision logic.
- **Config-driven decision artifacts** - Decision trees, decision tables, and scorecards load from JSON, separating business logic from code.
- **Runtime parameter tuning** - `param()` values can be adjusted per call via a params document, letting business-owned thresholds change without redeployment.
- **Multiple execution modes** - Pipelines run interpreted or compiled with numba, and can be paused/stepped through in a debugger for rule-by-rule inspection.
- **HTTP serving and CLI** - Built-in server (uvicorn/starlette or sanic) and CLI commands for scaffolding, building/warming config versions, and serving pipelines.
- **AI agent tooling** - A Claude Code plugin provides a skill and MCP server for reading and editing pipelines, trees, tables, scorecards, and params with validation.
- **Optional symbolic proofs** - An extra built on z3 can formally verify rule properties.

## Technology Stack
- **Languages:** Python (3.10+)
- **Dependencies:** polars (DataFrames), numba (compilation), uvicorn + starlette or sanic (serving), fastmcp (MCP server), z3-solver (optional proofs), uv (tooling), pytest (testing)
- **License:** MIT

## GitHub Resources
- [capitec/dsp-decision-engine](https://github.com/capitec/dsp-decision-engine) - Decision engine and visualization framework for building Python decision pipelines (decision trees, tables, scorecards)

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[jDMN - Java DMN Decision Engine for Executing and Translating Business Decision Models]]
