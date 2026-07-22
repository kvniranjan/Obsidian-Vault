---
date: 2026-07-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, spec-driven-development, ai-assisted, prd, specifications, sdlc, context-engineering]
source: GitHub
---

# OpenSpec - AI-Powered Spec-Driven Development Framework

## What is it?
OpenSpec is a spec-driven development (SDD) framework that structures the conversation between Business Analysts, product teams, and AI coding assistants before any code is written. It uses a lightweight Markdown-based workflow where a change is described, an AI drafts a short specification and task list, and both human and AI align on the plan before implementation begins. With over 62,000 stars and integrations for 25+ tools including Claude Code, Cursor, and AWS Kiro, it has become one of the most widely adopted specification frameworks in the AI-assisted development space.

## Why it matters for Business Analysts
OpenSpec closes the gap between BA requirements and developer execution by enforcing a structured specification step that produces traceable, human-readable artefacts stored alongside the codebase. Its "delta spec" model describes only what is changing rather than restating the entire system, which mirrors how BAs write change requests and impact assessments in iterative delivery. Because specs are plain Markdown with no proprietary syntax, BAs can author, review, and version them in any editor without tooling lock-in. The proposal-to-archive lifecycle (explore → propose → apply → archive) gives BAs a clear audit trail of every change's rationale, design, and resulting tasks, directly supporting traceability requirements.

## How to use it in BA Workflows
1. **Requirements Capture as Spec Proposals** - Use `/opsx:propose` to turn a stakeholder change request into a structured proposal containing a design document, specification files, and a task breakdown; review and refine these artefacts before any implementation begins.
2. **PRD and Feature Specification** - Author product requirements documents in OpenSpec's Markdown schema so AI coding assistants can consume them directly, reducing the translation loss between BA artefacts and developer tickets.
3. **Change Impact Analysis** - Leverage delta specs to document only the incremental change to existing functionality, keeping impact assessments concise and linked to the affected spec files for traceability.
4. **Iterative Refinement with AI** - Use `/opsx:explore` to interrogate the existing specification base and surface gaps or contradictions before committing to a proposal, effectively giving BAs an AI-assisted requirements review pass.
5. **Audit Trail and Archiving** - After implementation, `/opsx:archive` closes the change record and preserves the full proposal-to-implementation history in the repository, satisfying regulatory or governance requirements for documented change management.

## Key Features
- **Plain Markdown specs** — No proprietary DSL; all artefacts are human-readable `.md` files that work in any editor or wiki
- **Structured proposal workflow** — Single command generates design doc, specs, and task list from a natural-language change description
- **Delta spec model** — Describes only what changes rather than restating the entire specification, ideal for brownfield and evolving systems
- **25+ AI tool integrations** — Native support for Claude Code, Cursor, AWS Kiro, Pi.dev, and other AI coding assistants
- **Version-controlled artefacts** — Specs and proposals live in the repository alongside code, enabling full Git-based history and diffing
- **Schema validation** — Structured schemas for spec-driven artefacts ensure consistency across proposals and teams
- **Archive lifecycle** — Completed changes are archived with full provenance, supporting audit and compliance needs

## Technology Stack
- **Languages:** TypeScript
- **Dependencies:** Node.js / npm package (`@fission-ai/openspec`); integrates with any AI coding assistant via slash commands
- **License:** MIT

## GitHub Resources
- [Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec) - Spec-driven development (SDD) framework for AI coding assistants (62k+ stars)

## Related Skills
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
