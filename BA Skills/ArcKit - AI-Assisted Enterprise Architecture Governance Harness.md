---
date: 2026-11-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, decision-management, ai-assisted-ba, enterprise-architecture, traceability]
source: GitHub
---

# ArcKit - AI-Assisted Enterprise Architecture Governance Harness

## What is it?
ArcKit is an open-source toolkit that turns enterprise architecture governance — strategy, requirements, design, procurement, and assurance — into a structured, AI-assisted workflow instead of a pile of scattered Word and PowerPoint documents. It ships as a set of slash commands and templates for AI coding assistants (Claude Code, Gemini CLI, GitHub Copilot, Codex CLI) that draft reviewable governance artefacts and enforce traceability between them.

## Why it matters for Business Analysts
ArcKit directly automates core BA deliverables — requirements documents, stakeholder driver/goal/outcome analysis, business case justification, data models, and architecture decision records — while keeping every output as a `Status: DRAFT` artefact that a named accountable person must review and sign off. For BAs working alongside enterprise architects, it provides a consistent, version-controlled (Git-based) template library instead of ad-hoc documents, and it automatically flags gaps and coverage issues in requirements-to-design traceability, which is one of the most error-prone parts of a BA's job.

## How to use it in BA Workflows
1. **Requirements elicitation and drafting** - Run `/arckit:requirements` to generate a comprehensive requirements document from project context, keeping functional and non-functional requirements consistently structured.
2. **Stakeholder analysis** - Use `/arckit:stakeholders` to systematically capture stakeholder drivers, goals, and outcomes instead of building the matrix manually in a spreadsheet.
3. **Requirements traceability** - Run `/arckit:traceability` to maintain and automatically audit links between requirements, design decisions, and delivery artefacts, surfacing orphaned or unmapped requirements.
4. **Business case and decision management** - `/arckit:sobc` drafts a Strategic Outline Business Case (HM Treasury Green Book style) and `/arckit:adr` produces Architecture Decision Records, giving BAs a repeatable structure for justifying and recording decisions.
5. **Data modeling and diagrams** - `/arckit:data-model` and `/arckit:dfd` generate ERDs, data-flow diagrams, and Mermaid visuals directly from requirements text, reducing the gap between written requirements and process/data models.

## Key Features
- 73+ official slash commands covering the full governance lifecycle: principles, stakeholders, requirements, risk, business case, vendor RFP/evaluation, design review, and traceability.
- Enforced traceability with automatic gap detection between requirements, decisions, and design artefacts.
- Template-driven output so every artefact (requirements doc, ADR, DPIA, business case) follows a consistent, review-ready structure.
- Multi-platform: works as a Claude Code plugin, Gemini CLI extension, GitHub Copilot prompt set, or standalone Python CLI.
- Regional and sector overlays (UK Gov, NHS, EU, US, UAE and more) adding jurisdiction-specific compliance commands (GDPR, DPIA, AI Playbook, NCSC CAF).
- Explicit "what it does not do" guardrails — every artefact is marked DRAFT and routed to a named accountable reviewer, which keeps AI-generated BA output auditable rather than treated as final.

## Technology Stack
- **Languages:** Python (CLI), JavaScript/TypeScript (plugin tooling, Mermaid diagram generation)
- **Dependencies:** typer, rich, httpx, platformdirs (Python CLI); mermaid-cli, @antv/infographic (diagramming)
- **License:** MIT (core toolkit; one proprietary supplier overlay plugin is excluded from the MIT grant)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - Enterprise architecture governance harness with AI-assisted requirements, stakeholder analysis, traceability, and decision-management commands.

## Related Skills
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
