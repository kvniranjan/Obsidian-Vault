---
date: 2026-10-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, quality-assurance, functional-safety]
source: GitHub
---

# BASIL - Software Quality and Requirements Traceability Management Tool

## What is it?
BASIL (from the ELISA/elisa-tech open-source community) is a software quality management tool that lets teams break specifications or source code into snippets and link each one to requirements, test specifications, test cases, and test runs. It highlights traceability gaps, tracks completeness percentages across relationships, and exports full traceability matrices — originally built for functional-safety software but applicable to any requirements-heavy workflow.

## Why it matters for Business Analysts
BASIL gives BAs a structured, auditable way to prove that every requirement has been specified, implemented, and tested — closing the loop that spreadsheets and static RTMs struggle to maintain as projects evolve. The completeness percentages and automatic impact analysis mean a BA can immediately see which requirements are under-specified or under-tested after a scope change, instead of manually re-walking a traceability matrix. Granular read-only permissions let a BA share live traceability views with stakeholders or auditors without handing over edit rights, and bulk import/export (CSV, XLSX, YAML, JSON, SPDX) keeps it compatible with existing requirements documents and BRDs.

## How to use it in BA Workflows
1. **Requirements intake** - Import an existing BRD or requirements spreadsheet (CSV/XLSX) directly into BASIL as Software Requirement work items, preserving IDs for traceability.
2. **Traceability matrix maintenance** - Link each requirement to its corresponding test specifications and test cases, and let BASIL's completeness scoring flag requirements with no linked tests or documentation.
3. **Change impact analysis** - When a requirement changes, use BASIL's impact analysis to see every downstream specification, test, and document that is now out of date.
4. **Stakeholder reporting** - Export the traceability matrix to HTML or PDF for sign-off reviews, or give stakeholders read-only web access to the live matrix.
5. **AI-assisted requirement drafting** - Use BASIL's built-in OpenAI-powered suggestions to help draft or refine requirement and test-case wording directly in the work item editor.

## Key Features
- Work item types covering Software Requirements, Test Specifications, Test Cases, Test Runs, Justifications, and Documents
- Completeness percentage and gap detection on every traced relationship
- Impact analysis that flags downstream artifacts affected by a requirement change
- REST API for integrating traceability data into other toolchains
- Granular user permissions (e.g., read-only assessor roles) for safe stakeholder sharing
- Import from CSV/XLSX/YAML/JSON/SPDX and export of traceability matrices to HTML/PDF/SPDX
- In-app AI suggestions for drafting work items via the OpenAI API

## Technology Stack
- **Languages:** Python (API), JavaScript (App)
- **Dependencies:** Flask (backend), React + PatternFly (frontend), Cypress (testing), tmt/fmf (test metadata)
- **License:** GPL-2.0

## GitHub Resources
- [elisa-tech/BASIL](https://github.com/elisa-tech/BASIL) - Software quality management tool for tracing requirements, specifications, source code, and tests

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[rmToo - Git-Native Requirements Management Tool]]
