---
date: 2026-10-30
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-engineering, traceability, ai-assisted, mcp, git-native, decision-management]
source: GitHub
---

# Reqvire - Git-Native Semantic Requirements Engineering Framework

## What is it?
Reqvire is a Git-native semantic engineering framework for building verifiable, traceable software and systems. It models ontologies, capabilities, requirements, contracts, verification plans, and evidence as plain-text artefacts in a Git repository, then computes typed change-impact and coverage analysis across that model. It exposes its model through a CLI, a browser-based Explorer UI, and an MCP server so both engineers and AI assistants can navigate from business intent down to implementation.

## Why it matters for Business Analysts
Reqvire gives BAs a structured, version-controlled home for requirements that lives alongside the codebase instead of in a disconnected requirements tool, so every change to a requirement is reviewable in the same pull-request workflow as the code it governs. Its ontology and concept-scheme layer (SKOS-style terms, labels, synonyms, and definitions) doubles as a managed business glossary, keeping terminology consistent across stakeholders and documents. Because requirements, contracts, verification evidence, and implementation links are all typed and cross-referenced, BAs get automatic coverage and change-impact reports instead of hand-maintained traceability matrices. The built-in MCP server also lets AI coding assistants read and update the requirements model directly, which is increasingly how BA and engineering work is being bridged in AI-assisted delivery pipelines.

## How to use it in BA Workflows
1. **Requirements-as-Code Capture** - Author requirements, capabilities, and constraints as structured Markdown/model files committed to Git, so every requirement change goes through normal review and version history.
2. **Business Glossary via Ontologies** - Define concept schemes and concepts with labels, synonyms, and definitions to maintain a single source of truth for domain terminology across BA, product, and engineering teams.
3. **Traceability and Coverage Reporting** - Run `reqvire validate` and coverage reports to confirm every requirement links to a verification element and implementation artefact, replacing manual traceability-matrix upkeep.
4. **Change-Impact Analysis** - Use Reqvire's typed change-impact computation to see exactly which capabilities, contracts, and verification plans are affected before approving a requirement change.
5. **AI-Assisted Requirements Review** - Connect Claude Code or another MCP-compatible AI assistant to Reqvire's MCP server so it can query, lint, and (with mutations enabled) author or refine requirements under BA supervision.

## Key Features
- **Ontology and vocabulary modeling** — SKOS-style concept schemes and reusable SHACL-based semantic contracts for consistent terminology
- **Capabilities-to-requirements anchoring** — requirements refined with behavioral contracts, state models, I/O contracts, and constraints
- **Verification planning** — verification objectives and elements linked directly to requirements and evidence
- **Traceability, coverage, and change-impact analysis** — automated, typed reporting instead of manual matrices
- **Multi-repository support** — combines a Google Repo workspace with component repositories for large programs
- **MCP server integration** — typed tools, resources, and prompts over Streamable HTTP or stdio for AI-assistant workflows
- **Explorer UI** — browser-based visual navigation of the semantic model via `reqvire serve`

## Technology Stack
- **Languages:** Rust (core engine), with Node/npm distribution
- **Dependencies:** Distributed via shell installer or npm (`@reqvire-org/reqvire`); optional Hermit environment pins Rust, Node, Bun, Python, ripgrep, and Google Repo
- **License:** Apache 2.0

## GitHub Resources
- [reqvire-org/reqvire](https://github.com/reqvire-org/reqvire) - Git-native semantic requirements engineering framework with MCP support for AI assistants

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[OpenFastTrace - Requirements Traceability Suite]]
