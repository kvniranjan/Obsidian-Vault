---
date: 2026-10-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, business-rules, decision-tables, excel, requirements-management]
source: GitHub
---

# DTRules - Excel-Based Decision Table Rules Engine

## What is it?
DTRules is an open-source, Apache 2.0-licensed decision table rules engine that lets business analysts and policy experts author complex business logic directly in Excel spreadsheets rather than code. The engine compiles those spreadsheets into executable bytecode that runs on a lightweight, embeddable virtual machine, and it traces its lineage to real-world eligibility and audit systems (Texas TIERS, Ohio OFAST) with thousands of production decision tables.

## Why it matters for Business Analysts
Decision tables are one of the clearest ways to document conditional business logic (eligibility rules, pricing tiers, approval criteria, regulatory policy) in a format non-programmers can read and validate line by line. DTRules treats the Excel workbook itself as the system of record, so BAs own and maintain the actual rule logic — not just a specification handed off to developers for reimplementation. This closes a common gap in requirements-to-implementation handoff, where business rules captured in a BRD drift from what engineers eventually code. Because rules compile to a verifiable, testable artifact, BAs also get a repeatable way to validate "if X then Y" policy logic before it reaches production.

## How to use it in BA Workflows
1. **Policy and eligibility rule authoring** - Capture eligibility, entitlement, or approval criteria (e.g., benefits qualification, loan underwriting, discount tiers) as condition-action matrices in Excel, with each column representing one discrete, reviewable rule.
2. **Requirements-to-logic traceability** - Use the Excel rule sheets as a living, executable extension of the requirements document, so stakeholders can trace a business rule directly from the BRD/FRD into the artifact that actually runs in production.
3. **Decision logic validation and sign-off** - Run `dtrules verify` to catch mismatches between the Excel authoring layer and compiled logic before a release, giving BAs a lightweight UAT step for rule changes without needing a developer in the loop.
4. **Interactive requirements elicitation / interviews** - Deploy a rule set as a CLI or web "interview" (`--interactive` / `--web`) that walks a stakeholder through missing inputs, useful for eliciting structured decision criteria during workshops.
5. **Policy change impact analysis** - Because each rule set can run in batch mode against historical data (`dtrules run --input`), BAs can test how a proposed policy change (e.g., a new eligibility threshold) would have affected past cases before approving the change.

## Key Features
- **Excel-first authoring** - Business rules live in spreadsheets; `dtrules build` extracts and compiles them, so the spreadsheet stays the source of truth rather than generated code.
- **Compiled, verifiable execution** - Rules compile to postfix bytecode on a stack-based VM, giving deterministic, testable behavior instead of ad-hoc spreadsheet formulas.
- **Multiple front-ends from one rule set** - The same compiled logic can run as a batch job, a CLI interview, an HTTP API, or a web interview.
- **Self-contained deployment** - Compiled rules embed into a single Go binary with no external files needed at runtime, simplifying handoff from BA-authored logic to IT operations.
- **230+ built-in operators and a fixed-point numeric type** - Supports precise financial/eligibility math without floating-point drift.
- **Consistency checking** - `dtrules verify` flags drift between the Excel authoring layer and the compiled logic.

## Technology Stack
- **Languages:** Go (core engine, CLI, API server), TypeScript/React (visual authoring UI), archived Java implementation (`legacy/`)
- **Dependencies:** ANTLR-based Expression Language compiler, Excel⇆XML conversion toolchain
- **License:** Apache License 2.0

## GitHub Resources
- [dtrules/dtrules](https://github.com/dtrules/dtrules) - Decision table rules engine letting business analysts author rules in Excel and run them as batch jobs, CLI interviews, or web apps.

## Related Skills
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[jDMN - Java DMN Decision Engine for Executing and Translating Business Decision Models]]
