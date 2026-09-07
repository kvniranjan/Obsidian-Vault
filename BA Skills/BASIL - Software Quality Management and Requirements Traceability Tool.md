---
date: 2026-09-07
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, requirements-tracing, quality-management, ai-assisted]
source: GitHub
---

# BASIL - Software Quality Management and Requirements Traceability Tool

## What is it?
BASIL is an open-source software quality management tool built to define and maintain traceability matrices across the full requirements-to-code-to-test chain. It decomposes specifications (or source code directly) into traceable snippets and links each one to work items — requirements, test specifications, test cases, test runs, justifications, and documents — surfacing coverage gaps automatically. Born at Red Hat to support functional-safety certification, it now runs under the Linux Foundation's ELISA project and is actively maintained.

## Why it matters for Business Analysts
Traceability is a core BA deliverable, but keeping a requirements-to-test matrix current by hand is tedious and error-prone the moment implementation starts. BASIL automates that matrix, showing at a glance which requirements are covered, untested, or orphaned, and runs impact analysis so a change to one specification immediately flags every downstream work item that needs review. Its import/export support for SPDX, YAML, JSON, CSV, and XLSX lets BAs pull requirements from existing tools rather than re-authoring them, and its AI-assisted work item suggestions speed up decomposing large specs into granular, testable items. For regulated or safety-critical domains, BASIL's exportable traceability reports (HTML, PDF, SPDX SBOM) double as audit-ready evidence of requirements fulfillment.

## How to use it in BA Workflows
1. **Traceability Matrix Maintenance** - Import a specification or requirements document, decompose it into snippets, and link each snippet to test specs and test cases so the matrix stays synchronized as work items evolve.
2. **Coverage Gap Analysis** - Use BASIL's dashboards to identify requirements with no linked test coverage or design justification before a release, closing gaps proactively instead of during audit.
3. **Change Impact Assessment** - When a stakeholder requests a specification change, use BASIL's linked work-item graph to see every requirement, test, and document affected, producing a concrete scope for re-estimation.
4. **Requirements Import/Export** - Bring existing requirements in from CSV, XLSX, YAML, or SPDX exports of other tools, then export the resulting traceability matrix as HTML or PDF for stakeholder review or compliance sign-off.
5. **AI-Assisted Requirement Decomposition** - Use BASIL's OpenAI-backed suggestions to help break a large specification into well-scoped, individually traceable requirement items, reducing manual authoring effort.

## Key Features
- **Specification decomposition** — splits documents or source code into traceable snippets mapped to work items
- **Multi-type work items** — requirements, test specifications, test cases, test runs, justifications, and documents in one traceability graph
- **Test infrastructure integration** — runs and traces tests from containers, VMs, and physical hardware, plus external CI (GitHub Actions, GitLab CI, KernelCI, Testing Farm, LAVA)
- **SPDX SBOM export/import** — exports a Design SBOM (SPDX Model 3) and imports requirements from SBOM sources
- **Impact analysis** — flags every downstream work item affected when a specification changes
- **REST API** — integrates traceability data into external pipelines and dashboards
- **AI-powered suggestions** — OpenAI-backed assistance for decomposing specifications into work items

## Technology Stack
- **Languages:** Python (Flask backend), JavaScript/React (Patternfly frontend)
- **Dependencies:** Flask, React, Patternfly, tmt (Test Management Tool), SPDX Model 3
- **License:** GNU General Public License v2.0

## GitHub Resources
- [elisa-tech/BASIL](https://github.com/elisa-tech/BASIL) - Software quality management tool for requirements traceability, work item tracking, and gap analysis

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[CAIRIS - Security-Driven Requirements and Persona Modeling Platform]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
