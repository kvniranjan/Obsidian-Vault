---
date: 2026-04-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, version-control, documentation, open-source]
source: GitHub
---

# rmToo - Git-Native Requirements Management Tool

## What is it?
[rmToo](https://github.com/florath/rmtoo) is a free, open-source requirements management tool written in Python that stores all requirements as plain-text files (supporting both a custom `.req` format and YAML) inside a standard Git repository. It processes requirements and topic hierarchies from these files and generates multiple output artefacts: HTML documentation sites, LaTeX/PDF reports, traceability dependency graphs (via Graphviz), statistical quality reports, and spreadsheet exports. Because everything lives in Git, the full history of every requirement — who changed it, when, and why — is automatically preserved.

## Why it matters for Business Analysts
rmToo solves the "requirements drift" problem that plagues shared-document or spreadsheet-based approaches: every requirement change is a Git commit with a message and author, giving BAs an immutable audit trail that satisfies compliance and governance requirements without extra process overhead. Plain-text storage means requirements integrate naturally with code review workflows (pull requests, diff views), letting developers and BAs review and approve requirement changes using the same tooling they use for code. The automated quality analytics feature statically checks each requirement for completeness (missing attributes like owner, priority, or acceptance criteria) and flags gaps before a review cycle — reducing the back-and-forth between BAs and stakeholders. Dependency graph generation makes traceability from business need to functional requirement to test case visual and verifiable.

## How to use it in BA Workflows
1. **Version-Controlled Requirements Baseline** — Store all BRD/FRS requirements as `.req` or YAML files in a Git repo; every sprint's baseline is a tagged commit, making rollback and change impact analysis trivial.
2. **Automated Traceability Matrix** — Define parent-child relationships between business requirements and functional requirements in the file metadata; rmToo generates a dependency graph that serves as the traceability matrix for audits.
3. **Requirement Quality Gate** — Run rmToo's quality analytics as a CI step (GitHub Actions / GitLab CI); any requirement missing a mandatory attribute (status, owner, priority) fails the pipeline and blocks merge, enforcing completeness before review.
4. **Change Impact Analysis** — Use `git log` and `git diff` on the requirements directory to produce a per-sprint change log showing exactly which requirements were added, modified, or removed and by whom.
5. **Multi-Format Documentation Generation** — Generate an HTML requirements portal for stakeholders, a PDF for sign-off, and a dependency graph for architecture review — all from the same source files with a single command.

## Key Features
- Plain-text requirements in `.req` (custom format) or YAML — fully diff-able and merge-able in Git
- Hierarchical topic structure for organizing requirements into chapters and sections
- Automated requirement quality analytics: checks for missing mandatory attributes and flags incomplete entries
- Multiple output formats: HTML, LaTeX/PDF, Graphviz dependency graphs, spreadsheet export, statistical reports
- Full requirement traceability through parent-child dependency declarations
- Git-native: requirement history, authorship, and change log come from Git for free
- YAML storage backend for easier tooling integration
- pip/PyPI installable; project template available for quick setup
- CI/CD friendly: runs headlessly, returns non-zero exit codes on quality violations

## Technology Stack
- **Language:** Python 3.10+
- **Installation:** pip (`pip install rmtoo`)
- **Output Dependencies:** LaTeX (for PDF), Graphviz (for dependency graphs), Jinja2 (for HTML)
- **Storage:** plain text `.req` files or YAML, inside any Git repository
- **License:** GNU GPL v3.0+

## GitHub Resources
- [florath/rmtoo](https://github.com/florath/rmtoo) — Core requirements management tool and documentation

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[PM Tools Templates - Comprehensive BA Template Library]]
- [[Stakeholder Analysis Framework]]
- [[dmnmd - DMN Decision Tables in Markdown]]
