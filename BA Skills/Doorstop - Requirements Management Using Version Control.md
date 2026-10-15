---
date: 2026-10-15
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, traceability, version-control, documentation]
source: GitHub
---

# Doorstop - Requirements Management Using Version Control

## What is it?
Doorstop is an open-source requirements management tool that stores textual requirements as YAML files directly inside a version control repository (Git, SVN, Mercurial, Bazaar), alongside the source code they describe. Requirements are organized into documents, which are linked together into a traceable tree, and the tool validates that every parent-child link and reference stays consistent as the project evolves.

## Why it matters for Business Analysts
Doorstop lets BAs manage requirements the same way engineers manage code: diffable, reviewable in pull requests, and versioned with full history, instead of being locked away in a proprietary RM tool or a spreadsheet that drifts out of sync with delivery. Because requirements live next to the code and tests they govern, traceability from business need to implementation to test case is enforced automatically rather than maintained by hand in a traceability matrix. It is especially valuable for regulated or safety-critical domains (aerospace, medical, automotive) where auditors need evidence that every requirement is covered, but it works just as well for any BA practice that wants lightweight, Git-native requirements traceability without heavyweight tooling.

## How to use it in BA Workflows
1. **Structured requirements documents** - Create a document per requirements level (e.g., stakeholder requirements, system requirements, software requirements) using `doorstop create`, giving each a prefix so items are addressable (e.g., SRD001).
2. **Parent-child traceability** - Link child documents to parents (e.g., link software requirements to system requirements) so Doorstop can validate and visualize the full requirements hierarchy and flag orphaned or broken links.
3. **Review and sign-off tracking** - Mark items as reviewed after stakeholder sign-off; Doorstop detects when a reviewed item's content changes and flags it for re-review, supporting formal BA change-control processes.
4. **Traceability to tests** - Link requirement items to test case items in a separate document tree, giving BAs and QA a verifiable mapping from business need to test coverage for acceptance and compliance reporting.
5. **Publish stakeholder-facing documents** - Use `doorstop publish` to export the requirements tree to HTML, Markdown, or plain text, producing a readable, versioned requirements specification for stakeholder review without manual reformatting.

## Key Features
- YAML-based requirement items, human-readable and diff-friendly in any VCS
- Document tree model with enforced parent-child linking and automatic integrity validation
- CLI and Python API for scripting bulk edits, imports, and custom reporting
- Change detection on reviewed/approved items to support formal sign-off workflows
- Publishing to HTML, Markdown, and plain text for stakeholder-readable output
- VCS-agnostic: works with Git, Subversion, Mercurial, and Bazaar

## Technology Stack
- **Languages:** Python
- **Dependencies:** Python 3.9+, a supported version control system (Git/SVN/Mercurial/Bazaar), PyYAML, Jinja2 (for publishing)
- **License:** LGPLv3

## GitHub Resources
- [doorstop-dev/doorstop](https://github.com/doorstop-dev/doorstop) - Requirements management using version control

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[OpenFastTrace - Requirements Traceability Suite]]
