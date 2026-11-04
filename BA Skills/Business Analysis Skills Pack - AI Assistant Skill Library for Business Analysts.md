---
date: 2026-11-04
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements, elicitation, stakeholder-analysis, prioritization, claude-skills]
source: GitHub
---

# Business Analysis Skills Pack - Platform-Neutral AI Assistant Skills for BAs

## What is it?
`business-analysis-skills` is an MIT-licensed, platform-neutral library of 53 Markdown-based "skills" that teach AI assistants (Claude, Codex, and other agent frameworks) how to perform classic business analysis techniques and workflows. Rather than being a standalone application, it is a drop-in instruction pack: each skill is a `SKILL.md` file that an AI agent loads to run a specific BA method correctly and consistently.

## Why it matters for Business Analysts
This repo packages decades of BA methodology (PESTLE, SWOT, MoSCoW, RACI, stakeholder registers, interview/workshop design, use-case specification, traceability, and more) into reusable prompts an AI assistant can execute reliably instead of improvising. For BAs already using Claude Code, Codex, or similar agents, it turns ad-hoc AI help into a repeatable, auditable BA toolkit covering elicitation, specification, and quality review. It's especially useful for solo BAs or small teams who want consulting-grade rigor (bias checks, ambiguity detection, gap audits) without licensing a full BA suite, and it directly demonstrates the "AI-assisted BA workflow" pattern that's increasingly expected on BA teams.

## How to use it in BA Workflows
1. **Business problem framing** - Run the framing workflow skill at project kickoff to turn a vague ask into a structured problem statement with scope, objectives, and constraints before any requirements work starts.
2. **Stakeholder analysis** - Use the stakeholder register and RACI/RASCI skills to identify, map, and assign responsibility to stakeholders for a new initiative, producing a ready-to-share stakeholder matrix.
3. **Requirements elicitation** - Apply the interview and workshop design skills to generate structured elicitation plans and probing questions, then feed session notes into the elicitation workflow to extract business rules and assumptions.
4. **Requirements specification and packaging** - Use the acceptance-criteria, conflict-checking, and traceability skills to turn raw notes into clean requirements, then run the requirements packager workflow to assemble a delivery-ready requirements pack.
5. **Quality review before handoff** - Run the bias, evidence-gap, and requirements-quality check skills as a final pass before requirements go to development, catching ambiguity and inconsistency early.

## Key Features
- 53 skills organized into four tiers: atomic techniques (17), requirements/specification (14), elicitation/process extensions (10), and quality checks (5), plus 7 multi-step workflows
- Classic BA frameworks included as skills: PESTLE, SWOT, Porter's Five Forces, MoSCoW prioritization, RACI/RASCI, use-case specification
- Multi-step workflow skills chain atomic techniques together (e.g., stakeholder analysis, requirements elicitation, requirements packaging)
- Reusable BA templates under `docs/ba/templates/` for consistent deliverables
- Simple install/uninstall shell scripts that deploy skills globally (`~/.claude/skills/`, `~/.agents/skills/`) or per-project
- Platform-neutral design: works with Claude Code, Codex, and other agent frameworks that support Markdown skill files

## Technology Stack
- **Languages:** Markdown (skill definitions and templates), Shell (install/uninstall scripts)
- **Dependencies:** None beyond a compatible AI coding agent (Claude Code, Codex, or similar) that supports Markdown skill files
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Platform-neutral BA skill pack for AI assistants covering requirements, elicitation, stakeholder analysis, process work, and prioritization

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
