---
date: 2026-08-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-engineering, enterprise-architecture, traceability, ai-assisted, compliance, governance, claude-code]
source: GitHub
---

# ArcKit - AI-Assisted Enterprise Architecture and Requirements Governance Platform

## What is it?
ArcKit is an open-source toolkit that turns enterprise architecture and requirements governance from scattered documents into systematic, AI-assisted workflows. It guides teams through structured delivery phases — stakeholder analysis, business case justification, requirements capture, design review, and compliance assessment — producing draft governance artefacts for qualified practitioners to review and approve. It runs as a plugin for Claude Code and other AI coding assistants (Gemini CLI, GitHub Copilot, Codex/OpenCode, Mistral Vibe, Kimi Code).

## Why it matters for Business Analysts
BAs are routinely responsible for stitching together stakeholder drivers, business goals, requirements, design decisions, and test coverage into a coherent, auditable trail — work that is normally manual and error-prone across spreadsheets and wikis. ArcKit automates that traceability infrastructure, flags gaps automatically, and drafts the supporting documents (principles, requirements, risk registers, compliance assessments) so the BA can focus on validation rather than formatting. Its multi-jurisdictional compliance overlays (GDPR, NIS2, AI Act, UK GDS Service Standard, and more) make it especially valuable for BAs working in regulated sectors like government, finance, and healthcare, where regulatory traceability is a hard deliverable, not a nice-to-have.

## How to use it in BA Workflows
1. **Stakeholder-to-requirements traceability** - Capture stakeholder drivers and business goals, then let ArcKit maintain automatic linkage down to requirements, design decisions, and test coverage, with gap detection when a link is missing.
2. **Requirements engineering with AI drafting** - Generate draft requirements, user stories, and backlog items (exportable to CSV for Jira/Azure DevOps or Trello) from stakeholder context, then refine and approve them as a qualified reviewer.
3. **Business case and strategic planning** - Use the bundled Strategic Outline Business Case (SOBC), Wardley mapping, and capability maturity templates to justify and scope a transformation initiative before requirements work begins.
4. **Compliance and regulatory assessment** - Run structured compliance assessments against frameworks like GDPR, NIS2, the EU AI Act, or the UK GDS Service Standard, producing draft artefacts a compliance officer or DPO can review and sign off.
5. **Vendor procurement support** - Generate RFPs, search G-Cloud/Digital Marketplace listings, and score vendor responses against evaluation criteria drafted from the captured requirements.

## Key Features
- Template-driven governance: standardized templates for principles, requirements, data models, risk registers, and compliance assessments
- Traceability infrastructure with automatic linkage between stakeholder drivers, goals, requirements, design decisions, and tests, plus gap detection
- Multi-jurisdictional compliance overlays: UK (GDS, NCSC CAF, MOD JSP 936), EU (GDPR, NIS2, AI Act, DORA, CRA, DSA), France, Canada, UAE, Austria, Netherlands, Australia, and NHS clinical safety
- AI-assisted drafting across multiple assistants (Claude Code, Gemini CLI, GitHub Copilot, Mistral Vibe, Kimi Code)
- Data governance tooling: ERD generation with GDPR mapping, DPIA support, and external data sourcing
- Explicitly produces DRAFT artefacts for qualified human review, not final legal/regulatory/clinical sign-off

## Technology Stack
- **Languages:** Python (arckit-cli, Hatch build system)
- **Dependencies:** Bundled MCP servers (AWS Knowledge, Microsoft Learn, Google Developer Knowledge, GovRepoScrape, UK Tenders); outputs in Markdown, JSON, Mermaid, CSV, YAML
- **License:** MIT (core plugin and most overlays); the UK G-Cloud supplier bid overlay is proprietary and Claude Code-only

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - The Enterprise Architecture Governance Harness for strategy, architecture, delivery, and assurance using AI coding assistants

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
