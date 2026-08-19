---
date: 2026-08-19
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-elicitation, formal-methods]
source: GitHub
---

# FRET - NASA's Formal Requirements Elicitation Tool

## What is it?
FRET (Formal Requirements Elicitation Tool) is an open-source desktop application developed by NASA Ames Research Center for writing, formalizing, and validating system requirements. It lets analysts author requirements in restricted, structured English and automatically generates parallel representations of each one — natural language, formal logic, and visual diagrams — so technical and non-technical stakeholders can all verify the same requirement means what they think it means.

## Why it matters for Business Analysts
BAs routinely write requirements that are later found to be ambiguous, untestable, or contradictory only after development starts. FRET forces requirements into an unambiguous, structured form at authoring time, catching vagueness, conflicts, and missing conditions before they become costly rework. Its hierarchical organization and automatic consistency checking make it well suited for large, complex requirement sets where manual review can't reliably catch cross-requirement conflicts. Because every requirement is expressed in plain restricted English alongside its formal representation, BAs can bridge the gap between business stakeholders (who read the English) and engineers (who need precision), without needing to learn formal logic themselves.

## How to use it in BA Workflows
1. **Structured requirements elicitation** - Capture requirements from stakeholder interviews directly into FRET's guided restricted-English templates, which nudge authors toward unambiguous phrasing (clear scope, condition, timing, and response) instead of free-text prose.
2. **Ambiguity and conflict detection** - Run FRET's consistency checker across a requirement set to surface contradictions or gaps (e.g., two requirements that can never both be satisfied) before handing specs to development or QA.
3. **Multi-audience requirement review** - Use the generated natural-language and diagram views in stakeholder walkthroughs, while engineers work from the same requirement's formal logic representation — eliminating "translation" errors between business and technical specs.
4. **Test coverage planning** - Leverage FRET's automated test-case generation to derive acceptance criteria and test scenarios directly from formalized requirements, tightening the link between requirements and QA.
5. **Requirements hierarchy management** - Organize large requirement sets into hierarchical levels (system, subsystem, component) to keep traceability clear on complex programs, similar to how BAs decompose epics into features and stories.

## Key Features
- Restricted natural-language requirement authoring with guided templates
- Automatic generation of formal logic and visual diagram representations per requirement
- Hierarchical organization of requirements across multiple levels
- Automated consistency checking to detect conflicting or contradictory requirements
- Automated test case generation with coverage metrics
- Export to external formal analysis and verification tools
- Cross-platform desktop app (macOS, Linux, Windows)

## Technology Stack
- **Languages:** JavaScript/TypeScript (Electron application)
- **Dependencies:** Electron, Node.js
- **License:** Apache License 2.0

## GitHub Resources
- [NASA-SW-VnV/fret](https://github.com/NASA-SW-VnV/fret) - NASA's formal requirements elicitation, specification, and analysis tool

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
