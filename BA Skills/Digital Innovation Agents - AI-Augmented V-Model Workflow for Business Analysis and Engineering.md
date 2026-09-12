---
date: 2026-09-12
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-engineering, claude-code-skills, v-model, process-modeling]
source: GitHub
---

# Digital Innovation Agents - AI-Augmented Business Analysis and Requirements Engineering Workflow

## What is it?
Digital Innovation Agents is an open-source skill pack that pairs a structured innovation methodology with an AI coding workflow, guiding AI assistants (Claude Code, Cursor, Codex, OpenCode, Gemini CLI, GitHub Copilot) through a six-phase V-Model: Business Analysis, Requirements Engineering, Architecture, Coding, Testing, and Security Audit. Each phase is quality-gated, so an AI assistant cannot jump straight to code without first producing evidence-backed discovery and requirements artifacts.

## Why it matters for Business Analysts
It formalizes AI-assisted BA work instead of leaving it to ad-hoc prompting: the Business Analysis phase runs structured discovery to capture users, needs, insights, and critical hypotheses, and proposes field research methods (interviews, persona synthesis, TRIZ, pre-mortem, wizard-of-oz) when existing answers are insufficient. It keeps a living BACKLOG.md and auto-updated ADRs as the single source of truth, so requirements traceability survives into architecture, coding, and testing rather than going stale after the kickoff meeting. For BAs partnering with AI-augmented delivery teams, it gives a repeatable handoff contract (tracked via git commit trailers) between the analysis phase and everything downstream.

## How to use it in BA Workflows
1. **Structured Discovery** - Run the `business-analysis` skill to elicit users, needs, and hypotheses using one of 32 built-in innovation/research techniques rather than freeform interviewing.
2. **Requirements Engineering Handoff** - Feed discovery outputs into the `requirements-engineering` skill to produce structured, testable requirements that quality-gate before architecture work begins.
3. **Reverse-Engineering Existing Systems** - Use the `dia-migration`/reverse-engineering entry points to walk the V-Model backwards over a legacy codebase, generating an evidence-based BA draft, feature inventory, and backlog seed with every claim sourced to code.
4. **Living Backlog Maintenance** - Treat `BACKLOG.md` and the auto-generated ADRs as continuously updated requirements documentation instead of a one-time deliverable, keeping stakeholders aligned as implementation evolves.
5. **Cross-Tool Governance** - Apply the same BA discipline across whichever AI coding assistant a team standardizes on, since the skills are portable across Claude Code, Cursor, Codex, OpenCode, Gemini CLI, and Copilot.

## Key Features
- **V-Model workflow** - Six sequential, quality-gated phases (BA, requirements engineering, architecture, coding, testing, security audit) prevent AI assistants from skipping analysis.
- **Thirteen skills** - Six phase skills plus foundation skills (project-conventions, consistency-check, humanizer, dia-bootstrap, dia-guide) for governance and tone.
- **32 innovation/discovery techniques** - Built-in library of research methods (interviews, persona synthesis, TRIZ, pre-mortem, wizard-of-oz) surfaced automatically when evidence is thin.
- **Reverse-engineering entry point** - Generates plan-context, ADRs, arc42 architecture docs, feature inventory, and a sourced BA draft from an existing codebase.
- **Git-trailer tracked handoffs** - Phase transitions are recorded as git commit trailers, giving an auditable trail from requirement to shipped code.
- **Multi-assistant portability** - Works across Claude Code, Cursor, Codex, OpenCode, Gemini CLI, and GitHub Copilot.

## Technology Stack
- **Languages:** JavaScript/Node.js (tooling), Python (helper scripts: flow.py, anchor.py)
- **Dependencies:** Claude Agent SDK / Claude Code Skills framework, npm tooling
- **License:** MIT

## GitHub Resources
- [pssah4/digital-innovation-agents](https://github.com/pssah4/digital-innovation-agents) - AI-augmented V-Model workflow connecting business analysis and software engineering through quality-gated Claude Code/Copilot/Cursor skills.

## Related Skills
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
