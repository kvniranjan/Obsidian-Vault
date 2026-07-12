---
date: 2026-07-12
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-engineering, plaintext, version-control, traceability, dsl, automotive]
source: GitHub
---

# TRLC - Treat Requirements Like Code with a Domain-Specific Language

## What is it?
TRLC is an open-source domain-specific language (DSL) and toolchain developed by BMW Software Engineering for writing, linking, and validating requirements in plain text files. Requirements are expressed in `.rsl` (schema) and `.trlc` (requirement) files that live alongside source code in version control. The Python-based toolchain validates requirements for type correctness and custom business rules, and exposes an API for building downstream tools like renderers, diff engines, and traceability reports.

## Why it matters for Business Analysts
TRLC closes the gap between requirements authoring and engineering rigor by storing requirements as structured, version-controlled text — making them reviewable via pull requests, diffable across releases, and traceable to tests and code. BAs working in regulated or safety-critical industries (automotive, aerospace, medical) benefit from automatic validation that catches incomplete or inconsistent requirements before they reach development. Because requirements are plain text, they integrate naturally into CI/CD pipelines, enabling quality gates on requirement health just like code quality. The companion BMW project LOBSTER extends this by linking requirements to software artefacts, models, and verification activities, giving BAs full traceability chains.

## How to use it in BA Workflows
1. **Requirements authoring** - Define a schema (`.rsl` file) capturing your requirement types, attributes, and custom validation rules, then write requirements in `.trlc` files using that schema; TRLC enforces attribute completeness and type correctness automatically.
2. **CI/CD quality gating** - Add `trlc lint` as a CI step on every pull request so the pipeline rejects malformed, missing, or rule-violating requirements before they reach Sprint planning or development handoff.
3. **Impact and change analysis** - Use the Python API to diff requirements between two releases, identifying added, modified, or deleted requirements to generate a structured change log for stakeholder review or regulatory submission.
4. **Traceability reporting** - Build or use LOBSTER alongside TRLC to link each requirement to its implementing code, tests, or models, then generate traceability matrices that satisfy audit demands or Definition-of-Done checklists.
5. **Requirements rendering** - Use the TRLC Python API to render requirements into HTML, PDF, or Confluence-compatible formats for stakeholder review, keeping the single source of truth in version control while producing readable artefacts on demand.

## Key Features
- **Domain-specific language** - Strongly typed `.rsl` schema files define requirement types and mandatory attributes; `.trlc` files hold actual requirement instances
- **Static analysis engine** - Validates requirements at parse time and enforces user-defined check rules, catching errors before they propagate
- **Python API** - Programmatic access to the parsed requirement tree for building renderers, diff tools, impact analysers, or custom exporters
- **Version control native** - Plain-text files work with any git workflow; requirements are reviewed, branched, and tagged like code
- **Bazel support** - First-class Bazel build integration for teams using monorepo setups in automotive or embedded environments
- **LOBSTER integration** - Pairs with BMW's LOBSTER tool for full requirements-to-verification traceability chains

## Technology Stack
- **Languages:** Python
- **Dependencies:** Python 3.8+; optional Bazel for build integration
- **License:** GNU General Public License v3.0 (GPL-3.0)

## GitHub Resources
- [bmw-software-engineering/trlc](https://github.com/bmw-software-engineering/trlc) - Domain-specific language and toolchain for treating requirements like code

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
