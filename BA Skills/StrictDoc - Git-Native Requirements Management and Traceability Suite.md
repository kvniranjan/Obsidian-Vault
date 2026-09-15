---
date: 2026-09-15
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-traceability, documentation-as-code, reqif]
source: GitHub
---

# StrictDoc - Git-Native Requirements Management and Traceability Suite

## What is it?
StrictDoc is an open-source software system for writing technical documentation and managing requirements as plain-text `.sdoc` files under version control. It provides a document tree, a bidirectional traceability screen, and a traceability matrix that link requirements to parent/child requirements, source code, and test results. It is widely used in safety- and compliance-critical industries (automotive, aerospace, medical devices) that follow standards such as DO-178C, ECSS, and IEC 62443.

## Why it matters for Business Analysts
BAs who own requirements documentation get a diff-friendly, git-native alternative to heavyweight tools like DOORS or Polarion, with full version history and pull-request-based review of requirement changes. The built-in traceability matrix makes it easy to spot orphaned or broken links between business requirements, derived requirements, and verification evidence, which is a recurring pain point in audits and stakeholder sign-off. Because the document schema (fields, requirement types) is user-configurable, BAs can tailor the requirement grammar to match their organization's existing templates rather than forcing content into a rigid vendor format. ReqIF import/export also lets BAs exchange requirement sets with clients or vendors who use commercial RM tools.

## How to use it in BA Workflows
1. **Requirements capture** - Write business, stakeholder, and system requirements as structured `.sdoc` entries with UIDs, titles, and statements, keeping every requirement individually addressable and reviewable in git diffs.
2. **Traceability auditing** - Use the traceability matrix screen to verify every business requirement traces down to a system requirement, test case, or code reference before sign-off, catching coverage gaps early.
3. **Stakeholder review packages** - Export the requirements set to PDF (via LaTeX) or static HTML for formal delivery to stakeholders, steering committees, or regulatory reviewers who need a fixed, shareable document.
4. **Tool interoperability** - Import existing requirement sets from DOORS, Polarion, or other ReqIF-compliant tools, or export StrictDoc requirements back into ReqIF for partners who require a specific commercial toolchain.
5. **Change management** - Track every requirement edit through normal git history, branches, and pull requests, giving BAs an auditable log of who changed what requirement and why, without a separate change-control system.

## Key Features
- Plain-text `.sdoc` format that is diff-friendly and stored natively in git, enabling code-review-style approval of requirement changes
- Customizable document grammar so requirement types and fields can mirror an organization's existing BA templates
- Traceability matrix and deep-trace screens showing parent/child requirement links, source code references, and test coverage in one view
- Multi-format export: HTML, RST, PDF, Excel, JSON, SPDX, and bidirectional ReqIF for interoperability with DOORS/Polarion
- Local web server for interactive browsing of the document tree during reviews

## Technology Stack
- **Languages:** Python
- **Dependencies:** Python 3.10+, pip-installable; LaTeX for PDF export
- **License:** Apache License 2.0

## GitHub Resources
- [strictdoc-project/strictdoc](https://github.com/strictdoc-project/strictdoc) - Software for technical documentation and requirements management

## Related Skills
- [[rmToo - Git-Native Requirements Management Tool]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
- [[OpenFastTrace - Requirements Traceability Suite]]
