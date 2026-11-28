---
date: 2026-11-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, business-rules, decision-tables, python]
source: GitHub
---

# DSP Decision Engine (decikit) - Decision Tables, Trees, and Scorecards as Code

## What is it?
DSP Decision Engine is an open-source decision management framework published as the Python package `decikit`. It lets teams express decision logic — decision tables, decision trees, and scorecards — as JSON-defined artifacts that run inside composable Python pipelines, executing over single records or batched Polars DataFrames.

## Why it matters for Business Analysts
Decision tables, trees, and scorecards are exactly the artifacts BAs already use to document eligibility rules, pricing logic, risk scoring, and approval criteria — this tool turns those same documented structures into executable, testable logic instead of a static spec that drifts from the implementation. Tunable parameters can be adjusted per call through a params document, so analysts can retune thresholds (e.g., a credit score cutoff or discount tier) without engineering rebuilding or redeploying anything. Built-in versioning and step-through debugging give BAs a way to trace exactly which rule fired and why, which supports audit and compliance narratives for regulated decisions (lending, underwriting, fraud). It bridges the usual gap between "the BA's decision table" and "the engineer's if/else code" by making the table itself the source of truth.

## How to use it in BA Workflows
1. **Externalize decision tables from specs into runnable artifacts** - Convert a decision table in a requirements doc (e.g., loan approval criteria) into a JSON decision-table artifact that the engine executes directly, removing translation drift between spec and code.
2. **Model risk/eligibility logic as decision trees** - Represent multi-branch eligibility or triage logic (e.g., claims routing, KYC risk tiers) as a decision tree artifact and validate outputs against test cases the BA defines.
3. **Build and tune scorecards collaboratively** - Define a scorecard (e.g., credit risk or vendor-risk scoring) as a JSON artifact with weighted factors, then adjust weights via the params document during stakeholder review sessions without a code change.
4. **Batch-test decision logic against historical data** - Run the pipeline over a Polars DataFrame of historical cases to validate that new or revised rules produce the expected decisions before go-live, supporting UAT and regression testing of business rules.
5. **Trace and audit individual decisions** - Use the debug/step-through session to walk through exactly which rule, branch, or scorecard factor drove a specific outcome, useful for audit requests, dispute resolution, or explaining automated decisions to regulators or customers.

## Key Features
- **Pipelines from plain Python functions** - Function arguments name inputs and the function name names the output, keeping pipeline steps declarative and readable
- **Composable control flow** - `flow`, `dag`, `branch`, and `loop` primitives combine simple steps into full decision pipelines
- **JSON-defined decision artifacts** - Decision trees, decision tables, and scorecards are loaded from JSON rather than hardcoded, separating business logic from application code
- **Tunable parameters** - `param()` values can be changed at call time via a params document without rebuilding the pipeline
- **Dual execution modes** - Pipelines run interpreted for development or compiled with numba for production performance
- **Step-through debugging** - Pipelines can be paused and inspected step-by-step for traceability
- **CLI and serving tooling** - `guide`, `template`, `build`, and `serve` commands, with optional HTTP serving (Starlette/Sanic), an MCP server for AI agents, and symbolic proof support via z3

## Technology Stack
- **Languages:** Python (3.10+)
- **Dependencies:** Polars, optional extras for numba (compiled execution), Starlette/Sanic (HTTP serving), z3 (symbolic proofs), MCP server support
- **License:** MIT

## GitHub Resources
- [capitec/dsp-decision-engine](https://github.com/capitec/dsp-decision-engine) - Decision engine and visualization framework for building decision tables, trees, and scorecards as versioned, executable Python pipelines

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[jDMN - Java DMN Decision Engine for Executing and Translating Business Decision Models]]
