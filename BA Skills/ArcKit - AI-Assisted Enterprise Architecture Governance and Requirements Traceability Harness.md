---
date: 2026-08-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, decision-management, ai-assisted-ba, enterprise-architecture, traceability]
source: GitHub
---

# ArcKit - AI-Assisted Enterprise Architecture Governance and Requirements Traceability Harness

## What is it?
ArcKit is an open-source toolkit that turns scattered architecture and requirements documentation into systematic, AI-assisted governance workflows. It ships 75+ commands (built primarily as Claude Code plugins, with support for GitHub Copilot, Gemini CLI, and others) spanning strategy, business justification, requirements engineering, design review, procurement, and compliance.

## Why it matters for Business Analysts
ArcKit directly automates core BA deliverables: stakeholder analysis with driver/goal/conflict mapping, business case generation (using HM Treasury Green Book methodology), and requirement documentation with enforced bidirectional traceability from stakeholder drivers through business goals, requirements, design artifacts, and test cases. Its automated gap detection flags orphaned or uncovered requirements — a task BAs otherwise do manually in spreadsheets. Because it's AI-assisted but explicitly accountable (draft artifacts are marked for qualified human sign-off), it fits BA workflows that need speed without losing ownership of decisions.

## How to use it in BA Workflows
1. **Stakeholder Analysis** - Run stakeholder-analysis commands to capture drivers, goals, outcomes, and conflict/synergy mapping, producing a structured artifact instead of an ad-hoc slide or spreadsheet.
2. **Business Case Development** - Generate Strategic Outline Business Cases aligned to measurable stakeholder benefits, useful for BAs supporting investment or funding decisions.
3. **Requirements Traceability** - Document requirements with enforced links to stakeholder drivers and design artifacts, then use automated gap detection to catch requirements with no downstream design or test coverage.
4. **Backlog Generation** - Convert prioritized requirements into product backlogs using MoSCoW, then export to Jira, Azure DevOps, or Trello for agile delivery teams.
5. **Compliance-Aware Documentation** - Apply built-in UK/EU/sector-specific compliance overlays (GDS Service Standard, GDPR, AI Act) when writing requirements or design docs for regulated programs.

## Key Features
- 75+ phase-organized commands covering governance foundation through compliance
- Enforced bidirectional traceability: stakeholder drivers → goals → requirements → design → tests
- Automated gap detection for orphaned or uncovered requirements
- Citation tracking with fetch timestamps for external regulatory sources
- 13+ community-contributed jurisdictional/sectoral overlays (UK, EU, France, UAE, Canada, NHS) without forking the core
- Wardley mapping, roadmapping, and architecture decision record generation
- Export integrations to Jira, Azure DevOps, Trello, and ServiceNow

## Technology Stack
- **Languages:** Python (CLI), Markdown-based artifact generation, Mermaid diagrams, MARP presentations
- **Dependencies:** Python 3.8+, uv/pip, Claude Code (primary platform), optional AI platform SDKs, MCP servers (AWS Knowledge, Microsoft Learn, Google Developer)
- **License:** MIT (one overlay, `arckit-uk-gcloud`, is proprietary and Claude Code-only)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - The Enterprise Architecture Governance Harness for strategy, architecture, delivery, and assurance using AI coding assistants

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
