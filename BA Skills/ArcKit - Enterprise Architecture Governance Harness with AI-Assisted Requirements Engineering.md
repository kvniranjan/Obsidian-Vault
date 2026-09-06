---
date: 2026-09-06
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-engineering, traceability, stakeholder-analysis, ai-assisted-ba, enterprise-architecture, decision-management]
source: GitHub
---

# ArcKit - AI-Assisted Enterprise Architecture Governance and Requirements Harness

## What is it?
ArcKit is an AI-assisted governance harness that turns scattered architecture and requirements documents into a structured, version-controlled workflow driven through AI coding assistants (Claude Code, Gemini CLI, GitHub Copilot, Codex/OpenCode CLI). It ships 75+ commands covering strategy, requirements, procurement, design review, and compliance, each producing a governed, traceable Markdown artefact rather than a one-off AI response.

## Why it matters for Business Analysts
BAs spend much of their time turning stakeholder input into traceable requirements and then keeping that traceability intact as designs and vendors change — ArcKit automates exactly that chain. Its Stakeholder → Driver → Goal → Outcome model gives a repeatable elicitation method with built-in impact analysis, while its requirements engine generates business, functional, non-functional, integration, and data requirements with acceptance criteria in a consistent document format. Because every artefact carries a document-control header and a DRAFT status until a qualified human signs it off, it fits naturally into governance-heavy environments (public sector, regulated industries) where BAs must show provenance for every requirement. The built-in gap detection across requirements → design → procurement → test also gives BAs an automated way to catch orphaned or unimplemented requirements before they become audit findings.

## How to use it in BA Workflows
1. **Stakeholder and driver analysis** - Run the stakeholder/driver commands to capture who wants what and why, converting raw stakeholder input into SMART goals and measurable outcomes with documented rationale.
2. **Requirements elicitation and documentation** - Generate structured BR/FR/NFR/INT/DR requirement sets with acceptance criteria, using the `ARC-[project]-REQ-v[version]` document convention so every requirement is versioned and attributable.
3. **Traceability and impact analysis** - Use the traceability commands to trace requirements through design and test artefacts, and to run change-impact analysis whenever a stakeholder driver changes.
4. **Vendor and RFP support** - Use the procurement commands to build vendor evaluation frameworks and RFPs that score proposals directly against the documented requirements, keeping vendor selection defensible.
5. **Compliance and design-review packaging** - Attach DPIA, security assessment, and HLD/DLD review artefacts to the same requirement set so compliance reviewers and architects work from the same traceable source of truth as the BA.

## Key Features
- 75+ slash commands spanning strategy, requirements, data architecture, procurement, design review, and compliance
- Stakeholder/Driver/Goal/Outcome traceability chain with automated gap ("orphan requirement") detection
- Requirements generator for business, functional, non-functional, integration, and data requirement types
- 10+ autonomous research agents (Claude Code) for market research and vendor/data-source discovery via live web search and MCP servers
- Sector and regional overlays (NHS, UK G-Cloud, TOGAF ADM, France/Netherlands/Austria/Canada/USA/UAE) layered on the same core engine
- Static-site and `manifest.json` export so artefacts can be published and consumed programmatically

## Technology Stack
- **Languages:** Markdown (artefact format), YAML (frontmatter/config), Bash (automation), Python (CLI)
- **Dependencies:** `arckit` Python package (pip/uv installable), jq, git, MCP servers (AWS Knowledge, Microsoft Learn, Google Developer Knowledge, uk-tenders, govreposcrape)
- **License:** MIT for the core toolkit and most overlays (a UK G-Cloud supplier overlay is proprietary/Claude Code only)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - The Enterprise Architecture Governance Harness for strategy, requirements, delivery, and assurance using AI coding assistants

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
