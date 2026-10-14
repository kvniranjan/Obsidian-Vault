---
date: 2026-10-14
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, quality-assurance, safety-critical, decision-management]
source: GitHub
---

# BASIL - Software Quality and Requirements Traceability Platform

## What is it?
BASIL ("The FuSa Spice") is an open-source software quality management tool developed under the Linux Foundation's ELISA project. It lets teams break a software component specification or source code into traceable snippets, link work items (requirements, test specifications, test cases, test runs, justifications, and documents) to those snippets, and measure analysis completeness through a web UI and REST API.

## Why it matters for Business Analysts
BASIL operationalizes one of the hardest parts of requirements management: proving that every requirement is covered by a test, a justification, or a document, and surfacing the gaps where it isn't. Its impact-analysis view shows completeness percentages whenever a specification changes, which gives BAs a live traceability matrix instead of a static spreadsheet that goes stale. The built-in AI suggestions for work item design (via the OpenAI API) let BAs draft candidate requirements or test specs from source snippets rather than writing them from scratch, and the SPDX/SBOM-based export format makes it straightforward to hand a defensible traceability record to auditors, regulators, or downstream engineering teams.

## How to use it in BA Workflows
1. **Requirements traceability matrix maintenance** - Import requirements from CSV, XLSX, JSON, YAML, or SPDX, then trace each one to the specification snippet it covers, and export the resulting matrix as HTML, PDF, or an SPDX-based SBOM for stakeholder review.
2. **Gap and completeness analysis** - Use the impact-analysis view to see, as a percentage, how much of a specification is covered by requirements, test cases, or justifications, and prioritize elicitation work on the uncovered snippets.
3. **Change impact assessment** - When a specification or source snippet changes, let BASIL flag every linked work item (requirement, test, justification) that may now be stale, instead of manually re-reading the whole document.
4. **Collaborative review and sign-off** - Drive requirement and test-case review cycles through BASIL's lifecycle states (new, in progress, in review), comments, notifications, and to-do items, with granular read-only access for external assessors or auditors.
5. **AI-assisted requirement drafting** - Point BASIL's AI suggestion feature at a specification snippet to generate a first-draft requirement or test specification, then edit and approve it rather than starting from a blank page.

## Key Features
- Work item types covering software requirements, test specifications, test cases, test runs, test run configurations, justifications, and documents
- Web UI plus REST API for integrating traceability data into other toolchains
- Granular user permissions, including read-only roles for assessors and auditors
- Import from SPDX Model 3, JSON, YAML, CSV, and XLSX; export of traceability matrices as HTML, PDF, or SPDX-based SBOM
- Test infrastructure integration (via tmt) with KernelCI, Testing Farm, GitHub Actions, GitLab CI, and LAVA
- AI-generated work item suggestions through the OpenAI API
- Comments, notifications, and to-do items for cross-functional collaboration

## Technology Stack
- **Languages:** Python (Flask API backend), JavaScript/React with PatternFly (frontend)
- **Dependencies:** tmt (Test Management Tool) with fmf metadata, SPDX Model 3 for SBOM import/export
- **License:** GNU General Public License v2.0 (GPLv2)

## GitHub Resources
- [elisa-tech/BASIL](https://github.com/elisa-tech/BASIL) - Software quality management tool for requirements, test, and traceability tracking

## Related Skills
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[CAIRIS - Security-Driven Requirements and Persona Modeling Platform]]
- [[rmToo - Git-Native Requirements Management Tool]]
