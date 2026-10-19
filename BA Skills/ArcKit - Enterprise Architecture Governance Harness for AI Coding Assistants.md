---
date: 2026-10-19
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-engineering, enterprise-architecture, traceability, stakeholder-analysis, ai-assisted-ba, claude-code]
source: GitHub
---

# ArcKit - Enterprise Architecture Governance Harness

## What is it?
ArcKit is an open-source toolkit that turns AI coding assistants (Claude Code, Gemini CLI, GitHub Copilot, Codex CLI, and others) into an enterprise architecture and requirements governance harness. It ships as a plugin/command marketplace that generates versioned Markdown artefacts — requirements, business cases, risk registers, ADRs, design reviews, and traceability matrices — following established frameworks like TOGAF, MADR, and the HM Treasury Green Book.

## Why it matters for Business Analysts
BAs are regularly asked to produce requirements documents, stakeholder analyses, business cases, and traceability matrices that stay consistent and auditable across a project's lifecycle. ArcKit automates the drafting of these artefacts using an AI assistant while keeping every output as plain Markdown in Git, so requirements, decisions, risks, and stakeholders are version-controlled and diffable like code. Its `/arckit:traceability` command directly addresses a core BA pain point — proving that every requirement traces to a design element and a test, and flagging orphaned or unlinked items. The regional/sector overlays (UK Gov, NHS, finance, EU, TOGAF ADM) make it adaptable to regulated environments BAs often work in.

## How to use it in BA Workflows
1. **Requirements Elicitation and Documentation** - Use ArcKit's requirements commands to generate structured requirements documents with consistent ID schemes (BR, FR, NFR, INT, DR) straight from stakeholder notes or interview transcripts.
2. **Stakeholder and Business Case Analysis** - Run the stakeholder-driver and SOBC (Strategic Outline Business Case) commands to capture stakeholder goals, outcomes, and a Green Book-aligned business case the BA can hand to sponsors.
3. **Requirements Traceability Audits** - Use `/arckit:traceability` to auto-generate a matrix linking requirements to design and test artefacts, surfacing gaps before a review or audit.
4. **Risk and Decision Logging** - Generate an Orange Book-style risk register and MADR-based Architecture Decision Records so decisions affecting scope or requirements are documented alongside the requirements they impact.
5. **Backlog and User Story Generation** - Convert approved requirements into a prioritized backlog of user stories that developers can pick up directly, keeping requirements and delivery artefacts in sync.

## Key Features
- Command-driven generation of requirements, data models, business cases, risk registers, ADRs, HLD/DLD reviews, and roadmaps
- Built-in `/arckit:traceability` command producing requirement-to-design-to-test matrices with gap detection
- Mermaid/PlantUML diagram generation and inline citation markers for sourced claims
- Regional and sector overlay plugins (UK Government, EU, NHS, finance, TOGAF ADM, AI agent governance, and more)
- Markdown knowledge-bundle export/import (OKF format) for interoperability between projects
- Bundled MCP server integrations (AWS Knowledge, Microsoft Learn, UK tenders/gov scraping) for grounding artefacts in live sources
- Works across multiple AI coding assistants, not locked to a single vendor

## Technology Stack
- **Languages:** Python (CLI), Markdown (commands/templates/artefacts), Node.js tooling
- **Dependencies:** Claude Code plugin framework, MCP servers, Mermaid/PlantUML for diagrams, GitHub Actions/devcontainer for setup
- **License:** MIT (the `arckit-uk-gcloud` overlay is a proprietary exception)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - Enterprise Architecture Governance Harness driving strategy, architecture, delivery, and assurance through AI coding assistants

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
