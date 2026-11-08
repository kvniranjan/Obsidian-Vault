---
date: 2026-11-08
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, decision-management, data-analysis]
source: GitHub
---

# BASIL - Open-Source Requirements-to-Test Traceability and Safety Compliance Tool

## What is it?
BASIL (developed under the Linux Foundation's ELISA project) is an open-source web application for mapping software requirements to specifications, test cases, test runs, and source code, and for tracking how complete that coverage is. It ships a Python/Flask REST API and a React + PatternFly web UI, and it is built around traceability for safety-related ("FuSa") and quality-critical software, but the underlying workflow — requirement-to-test coverage mapping with gap analysis — applies to any regulated or quality-sensitive business domain.

## Why it matters for Business Analysts
Traceability matrices are a core BA deliverable, and BASIL automates the part that is normally a brittle spreadsheet: it links requirements to test specifications, test cases, and test runs, then computes a completeness percentage for every relationship so gaps in coverage are visible at a glance. Its impact-analysis feature flags downstream work items affected when a requirement changes, which directly supports change-impact assessment, a recurring BA responsibility. Granular, role-based permissions let a BA expose read-only traceability views to assessors, auditors, or stakeholders without giving them edit access, and built-in comments/notifications support the review-and-sign-off cycle BAs run with SMEs. The in-app AI suggestion feature (via the OpenAI API) also makes it a concrete example of AI-assisted requirements authoring inside a traceability tool.

## How to use it in BA Workflows
1. **Centralize requirements intake** - Import Software Requirements from SPDX Model 3 JSON, YAML, JSON, CSV, or XLSX, consolidating requirements gathered from multiple stakeholders or legacy documents into one traceable source.
2. **Build and visualize traceability matrices** - Map each requirement to Test Specifications, Test Cases, and source code snippets, then use the completeness percentage on each mapping to spot untested or unverified requirements before sign-off.
3. **Run change-impact analysis** - When a requirement or specification changes, use BASIL's impact analysis to see which linked test cases, test runs, and work items are affected, and apply suggested fixes to keep the matrix consistent.
4. **Coordinate review and sign-off** - Use work item lifecycle states (new, in progress, in review) plus comments and to-dos to run structured stakeholder review cycles, and grant assessors read-only access to the traceability views they need.
5. **Report coverage and compliance evidence** - Export the full traceability matrix as HTML, PDF, or an SPDX Model 3 "Design SBOM" to hand auditors, regulators, or leadership a defensible record of requirements coverage.

## Key Features
- Work item model covering Requirements, Test Specifications, Test Cases, Test Runs, Test Run Configurations, Justifications, and Documents
- Per-relationship completeness scoring to surface coverage gaps instantly
- Impact analysis with automated-fix suggestions when upstream specifications change
- Multiple mapping views so different teams can work the matrix in parallel
- Granular, role-based user permissions (e.g., read-only assessor access)
- Comments, notifications, and to-dos for collaborative review workflows
- Integration with external test infrastructure (tmt, KernelCI, Testing Farm, GitHub Actions, GitLab CI, LAVA)
- In-app AI suggestions for work item drafting via the OpenAI API
- REST API for embedding traceability data into other toolchains

## Technology Stack
- **Languages:** Python (Flask API), JavaScript/TypeScript (React + PatternFly frontend)
- **Dependencies:** tmt and fmf (test description/execution), OpenAI API (AI suggestions)
- **License:** GNU General Public License v2.0 (GPL-2.0)

## GitHub Resources
- [elisa-tech/BASIL](https://github.com/elisa-tech/BASIL) - Software quality management tool for requirements-to-test traceability, gap analysis, and compliance reporting

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[CAIRIS - Security-Driven Requirements and Persona Modeling Platform]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
