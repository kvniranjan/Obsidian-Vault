---
date: 2026-09-30
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, ai-assisted-ba, decision-management, enterprise-architecture]
source: GitHub
---

# ArcKit - Enterprise Architecture Governance Harness for AI-Assisted BA Workflows

## What is it?
ArcKit is an open-source "governance harness" that turns enterprise architecture and business analysis work into a systematic, AI-assisted workflow instead of scattered documents. It ships as a plugin/extension for AI coding assistants (Claude Code, Gemini CLI, GitHub Copilot, Codex, Kimi Code) and exposes 70+ slash commands covering strategy, requirements, design, delivery, and assurance activities, with the explicit philosophy of drafting artefacts "for qualified people to review" rather than auto-approving them.

## Why it matters for Business Analysts
BAs sit at the intersection of business need and technical delivery, and ArcKit packages many of the artefacts a BA is asked to produce — requirements documents, stakeholder analyses, business case justifications, RFP/vendor evaluation frameworks, and architecture decision records — as repeatable, AI-generated, version-controlled templates. Its traceability engine automatically maps requirements to design and flags gaps, which directly supports the BA responsibility of keeping requirements auditable end-to-end. Because it runs inside an AI coding assistant, a BA can draft governance-grade documentation conversationally and keep it in Git alongside the rest of the delivery record, rather than in disconnected Office documents. The regional/sector overlays (UK Government Service Standard, GDPR DPIA, NHS clinical safety, TOGAF ADM, etc.) also give BAs ready-made compliance and standards checklists to work against.

## How to use it in BA Workflows
1. **Requirements documentation** - Generate structured requirements documents from stakeholder input using the `/arckit-requirements` (or `arckit:requirements`) command, keeping requirements in Markdown/YAML under version control.
2. **Stakeholder analysis** - Run the stakeholder analysis workflow to identify, map, and document stakeholder interests and influence alongside the rest of an initiative's architecture artefacts.
3. **Requirements traceability** - Use the built-in traceability and gap-detection commands to verify every requirement maps to a design decision and every design decision cites a requirement, surfacing orphaned or unimplemented requirements automatically.
4. **Business case and decision management** - Draft business case justifications (Green Book SOBC-style) and architecture decision records (ADRs) so that key decisions and their rationale are captured as structured, searchable artefacts rather than meeting notes.
5. **Vendor/RFP evaluation** - Generate RFP documents and evaluation frameworks for build-vs-buy or vendor selection exercises, giving BAs a consistent scoring template for procurement decisions.

## Key Features
- **70+ slash commands** spanning strategy, architecture principles, requirements, data modeling (ERD), technology research, delivery, and assurance.
- **Automated traceability** - requirements-to-design mapping with automatic gap detection and citation tracking.
- **Governance templates** - risk management, business case justification, compliance assessment (GDPR DPIA, Secure by Design, service standards).
- **Strategic planning tools** - Wardley mapping, roadmapping, and architecture decision records built into the same workflow.
- **Regional/sector overlays** - installable add-ons for UK Government, EU (AI Act, NIS2, GDPR), Canadian federal, NHS, and finance-sector standards.
- **Multi-platform** - works as a plugin across Claude Code, Gemini CLI, GitHub Copilot, Codex CLI, and other AI coding assistants, so the same governance workflow travels with whichever AI tool a team already uses.

## Technology Stack
- **Languages:** Python (CLI), Markdown (templates/docs), YAML (configuration), Mermaid (diagrams)
- **Dependencies:** Distributed via `pip`/`uv` as a CLI (`arckit`), or installed as a native plugin/extension inside Claude Code, Gemini CLI, GitHub Copilot, and Codex/OpenCode CLI
- **License:** MIT (with a proprietary exception for the `arckit-uk-gcloud` supplier overlay)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - The Enterprise Architecture Governance Harness: strategy, architecture, delivery, and assurance using AI coding assistants

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[rmToo - Git-Native Requirements Management Tool]]
