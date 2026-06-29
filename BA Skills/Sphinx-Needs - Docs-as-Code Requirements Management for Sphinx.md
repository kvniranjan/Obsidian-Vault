---
date: 2026-06-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, documentation, traceability, sphinx, docs-as-code]
source: GitHub
---

# Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx

## What is it?
Sphinx-Needs is an open-source Sphinx extension that adds structured requirements, specifications, test cases, and design elements directly into plain-text documentation. It enables teams to define, link, and trace requirements within a docs-as-code workflow where all artifacts live in version control alongside code. It is widely adopted in safety-critical industries including automotive (ISO 26262), aerospace (DO-178C), and industrial (IEC 61508) domains.

## Why it matters for Business Analysts
BAs in regulated industries must maintain full traceability from business requirements through specifications to test cases — Sphinx-Needs makes this automatic rather than manual. Its docs-as-code model means requirements live in git, giving BAs full change history, branch-based review workflows, and pull-request approvals for every requirement change. The ability to define custom requirement types, link them bidirectionally, and auto-generate traceability matrices eliminates error-prone spreadsheet tracking. Because requirements, architecture docs, and compliance reports all live in one Sphinx project, stakeholder reviews pull from a single source of truth.

## How to use it in BA Workflows
1. **Define Custom Need Types** - Create types like `req`, `spec`, `story`, `test`, and `decision` to represent each artifact class in your BA process with their own mandatory fields and allowed status values
2. **Establish Bidirectional Traceability** - Use `:links:` and `:links_back:` directives to connect business requirements to functional specs and test cases, building a traceability matrix that updates automatically as docs evolve
3. **Generate Stakeholder Reports** - Use `needtable` to produce filtered tables of open requirements by status or owner, and `needflow` to render Graphviz diagrams showing dependency chains for review meetings
4. **Compliance Documentation** - Structure safety-critical requirement sets using built-in support for ISO 26262, DO-178C, and IEC 61508 patterns, generating compliant documentation packages for audits
5. **CI/CD Integration** - Run Sphinx builds in CI pipelines to validate requirement links are not broken and to publish living HTML documentation that always reflects the current state of requirements

## Key Features
- Custom need types with configurable fields, statuses, and layout templates
- Automatic bidirectional traceability matrix across all need types
- `needtable`, `needlist`, `needflow`, and `needpie` directives for filtered views and diagrams
- External needs: import requirements from other Sphinx-Needs projects for cross-team traceability
- Supports Graphviz and PlantUML for flow and dependency diagrams
- Full Sphinx ecosystem compatibility — PDF export, versioned docs, and theme support

## Technology Stack
- **Languages:** Python
- **Dependencies:** Sphinx, Graphviz (optional for flow diagrams), PlantUML (optional)
- **License:** MIT

## GitHub Resources
- [useblocks/sphinx-needs](https://github.com/useblocks/sphinx-needs) - Sphinx extension for structured requirements, traceability, and compliance documentation

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
