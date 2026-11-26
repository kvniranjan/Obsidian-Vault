---
date: 2026-11-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-elicitation, stakeholder-analysis, claude-skills]
source: GitHub
---

# Business Analysis Skills - Platform-Neutral AI Skill Pack for BAs

## What is it?
Business Analysis Skills (45ck/business-analysis-skills) is an open-source, platform-neutral collection of 53 reusable skills for AI coding/agent assistants, covering the full business analysis lifecycle from problem framing through requirements handoff and quality review. The skills are packaged as `SKILL.md` files compatible with Claude Code (`.claude/skills/`) and other agent tooling (`.agents/skills/`), and ship with reusable BA templates.

## Why it matters for Business Analysts
This repo turns classic BA techniques - PESTLE, SWOT, Porter's Five Forces, RACI, MoSCoW, CATWOE, stakeholder registers, use-case specs - into structured, invokable skills an AI assistant can run on demand, rather than knowledge the BA has to recall and apply manually each time. It bridges "AI-assisted BA workflows" directly: a BA can run `/stakeholder-analysis` or `/requirements-quality-check` as slash commands and get a consistent, technique-grounded output instead of an ad hoc LLM response. The built-in quality-check skills (evidence gaps, requirements quality, bias, assumption-checking) give BAs a repeatable self-review pass before handing deliverables to stakeholders or delivery teams, which is valuable for audit trail and consistency across a team using the same assistant.

## How to use it in BA Workflows
1. **Problem framing** - Run the business-problem-framing workflow skill at project kickoff to structure a vague ask into a scoped problem statement before requirements work starts.
2. **Stakeholder analysis** - Invoke the stakeholder-analysis workflow (backed by atomic RACI and stakeholder-register skills) to systematically map power/interest and communication needs.
3. **Requirements elicitation and packaging** - Use the elicitation workflow skills (interview design, probing questions, business rule extraction) to gather input, then the requirements-packaging workflow to assemble it into a structured deliverable.
4. **Process modelling (as-is/to-be)** - Apply the process-modelling workflow and as-is/to-be extension skills to document current and future-state processes ahead of BPMN diagramming.
5. **Quality review before handoff** - Run the requirements-quality-check and deliverable-consistency skills as a final gate, catching ambiguity, conflicting requirements, and unstated assumptions before sign-off.

## Key Features
- 53 skills across atomic techniques, requirements/specification, elicitation extensions, end-to-end workflows, and quality checks.
- Dual packaging for both `.claude/skills/` (Claude Code) and `.agents/skills/` (generic agent tooling), keeping the pack platform-neutral.
- Global install via `install.sh`/`uninstall.sh`, or per-project use by copying the skill folders.
- Reusable BA templates under `docs/ba/templates/` to pair with the skills' output.
- Slash-command style invocation (e.g. `/stakeholder-analysis`, `/requirements-quality-check`) for quick access inside an AI coding assistant.

## Technology Stack
- **Languages:** Markdown (`SKILL.md` definitions), Shell (install/uninstall scripts)
- **Dependencies:** None beyond a compatible AI agent/assistant (Claude Code or similar `.agents/skills/`-aware tooling)
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Platform-neutral business analysis skill pack for AI assistants, covering problem framing through requirements handoff and quality review.

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
