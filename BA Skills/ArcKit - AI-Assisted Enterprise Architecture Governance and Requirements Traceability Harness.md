---
date: 2026-08-20
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, requirements-management, traceability, ai-assisted, governance, wardley-mapping, procurement]
source: GitHub
---

# ArcKit - AI-Assisted Enterprise Architecture Governance and Requirements Traceability Harness

## What is it?
ArcKit is an open-source toolkit that wraps an AI coding assistant to transform enterprise architecture governance from scattered documents into a systematic, gated, and provenance-stamped workflow. It provides 70+ slash commands and agent skills for establishing architecture principles, authoring requirements, strategic planning with Wardley Mapping, running vendor RFP/selection, conducting formal design reviews (HLD/DLD), and maintaining end-to-end traceability. It runs across multiple AI platforms (Claude Code, Gemini CLI, GitHub Copilot, Codex, OpenCode, and others) producing identical, versioned Markdown artifacts.

## Why it matters for Business Analysts
ArcKit gives BAs a repeatable, AI-accelerated harness for the discovery-to-delivery lifecycle: it captures stakeholder drivers, goals, outcomes, and requirements and links them through design decisions to test coverage, so nothing falls between analysis and implementation. Its built-in traceability matrices, gap detection, and impact tracking directly answer the BA's recurring question of "which requirement drove this decision, and what breaks if it changes?" Because outputs are plain Markdown under version control, requirements and architecture decisions become reviewable, diff-able artifacts rather than stale wiki pages. The bundled compliance overlays (GDPR, UK Government TCoP/Service Standard, NHS, Finance) let BAs align requirements to regulatory frameworks without leaving their toolchain.

## How to use it in BA Workflows
1. **Requirements Elicitation & Documentation** - Use ArcKit's requirements commands to turn stakeholder interviews into structured requirement documents with unique IDs, acceptance criteria, and inline citation markers linking each requirement back to its source quote.
2. **Requirements Traceability Matrix** - Generate and maintain a traceability matrix connecting stakeholder drivers → goals → outcomes → requirements → design decisions → tests, then run gap detection to surface uncovered requirements before sign-off.
3. **Stakeholder & Strategic Analysis** - Apply the stakeholder analysis and Wardley Mapping skills to map who cares about what, position capabilities on the evolution axis, and justify build-vs-buy recommendations for a business case.
4. **Vendor RFP & Procurement Support** - Drive the vendor RFP authoring and selection commands to translate business requirements into evaluation criteria, score supplier responses, and produce an auditable selection rationale.
5. **Design Review & Impact Assessment** - Feed a proposed change into the HLD/DLD review and impact-tracking commands to see which requirements and downstream artifacts are affected, supporting change-control conversations with stakeholders.

## Key Features
- **AI-assisted command library** - 70+ slash commands / command-skills that generate architecture, requirements, and procurement artifacts across supported AI assistants.
- **End-to-end traceability** - Systematic linkage from stakeholder drivers through requirements and design decisions to test coverage, with gap detection and impact tracking.
- **Citation traceability** - Inline `[DOC-CN]` markers tie generated content to source documents with quoted evidence, giving BAs auditable provenance.
- **Wardley Mapping & strategic planning** - Built-in strategic-analysis skills for capability positioning, multi-year roadmaps, and build-vs-buy decisions.
- **Compliance overlays** - Regional and sector packs for UK Government (TCoP, Service Standard, Secure by Design), EU (GDPR, AI Act, NIS2), NHS, and Finance.
- **Multi-platform, versioned outputs** - Identical Markdown/YAML artifacts across Claude Code, Gemini CLI, Copilot, Codex, and OpenCode, all git-friendly.

## Technology Stack
- **Languages:** Python (CLI), Markdown (templates and outputs), YAML (configuration); JavaScript for supporting tooling
- **Dependencies:** Python 3.8+ with pip or uv; an AI coding assistant (Claude Code, Gemini CLI, GitHub Copilot, Codex, or OpenCode); Mermaid, PlantUML, ERD/C4, and Wardley Map rendering for diagrams
- **License:** MIT (core plugin and community overlays; the `arckit-uk-gcloud` supplier overlay is proprietary/Claude Code-only)

## GitHub Resources
- [tractorjuice/arc-kit](https://github.com/tractorjuice/arc-kit) - AI-harnessed enterprise architecture governance, requirements, and procurement toolkit for AI coding assistants.

## Related Skills
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[Stakeholder Analysis Framework]]
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
