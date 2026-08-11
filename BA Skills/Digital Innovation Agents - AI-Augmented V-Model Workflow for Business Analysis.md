---
date: 2026-08-11
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-engineering, discovery, claude-code, v-model]
source: GitHub
---

# Digital Innovation Agents - AI-Augmented V-Model Workflow for Business Analysis

## What is it?
Digital Innovation Agents is an open-source skill pack that pairs a structured business-analysis methodology with AI coding assistants (Claude Code, Cursor, GitHub Copilot, Codex, OpenCode, Gemini CLI). It walks a project through a six-phase V-Model — Business Analysis, Requirements Engineering, Architecture, Coding, Testing, and Security Audit — with quality-gated handoffs between each phase, so AI-driven delivery stays anchored to validated user needs instead of building the wrong thing quickly.

## Why it matters for Business Analysts
This is one of the few open-source tools built specifically to run *inside* an AI coding assistant as a first-class BA discipline rather than bolting BA on as an afterthought to code generation. The `/business-analysis` skill operationalizes a 32-method discovery catalog (interviews, extreme-user research, cultural probes, persona synthesis, stakeholder maps, jobs-to-be-done, pre-mortems, value-proposition quantification) with method cards explaining when to use each technique. The `/requirements-engineering` skill then enforces a clean separation between tech-agnostic user-observable requirements and downstream architectural decisions — directly addressing the common BA pain point of specs polluted with implementation detail. Because artifacts are recorded as living documents tied to git commit trailers, requirements traceability is maintained automatically as the build evolves.

## How to use it in BA Workflows
1. **Structured discovery on greenfield initiatives** - Run `/business-analysis` to conduct an Exploration → Ideation → Validation cycle, producing a condensed BA record and an exploration board (scope-adaptive: minimal for a quick test, full 10-section board for an MVP).
2. **Requirements drafting with enforced separation of concerns** - Use `/requirements-engineering` to convert discovery findings into epics/features (FEAT-EE-FF identifiers), tech-agnostic success criteria, and user stories spanning functional, emotional, and social dimensions.
3. **Reverse-engineering BA artifacts for existing systems** - On brownfield projects, run `/dia-realign` to reverse-walk an existing codebase and reconstruct the missing BA/requirements documentation.
4. **Workflow triage and onboarding** - Use `/dia-guide` to audit current project state and get a recommendation for which phase/skill to run next.
5. **Stakeholder-ready traceability** - Reference the git commit trailers (`DIA-Phase`, `DIA-Handoff`, `DIA-Triage`) to show stakeholders and auditors a clear, phase-by-phase chain from user problem through requirements, architecture, code, tests, and security review.

## Key Features
- 32-method discovery catalog with method cards (technique, team composition, common failure modes)
- Scope-adaptive rigor — same methodology, from a few-hour "Simple Test" up to a full multi-month MVP
- Tech-agnostic requirements enforcement (no implementation vocabulary allowed in user-facing success criteria)
- Living documentation — ADRs, features, architecture docs, and backlog update continuously during implementation
- Cross-tool support: works identically across Claude Code, Cursor, Copilot, Codex, OpenCode, and Gemini CLI

## Technology Stack
- **Languages:** JavaScript (skill/plugin tooling)
- **Dependencies:** Distributed as a Claude Code plugin marketplace / skill pack; no external service required
- **License:** MIT

## GitHub Resources
- [pssah4/digital-innovation-agents](https://github.com/pssah4/digital-innovation-agents) - AI-augmented V-Model workflow connecting business analysis and software engineering into one skill set

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
