---
date: 2026-10-04
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-management, elicitation, stakeholder-analysis, claude-skills]
source: GitHub
---

# Business Analysis Skills - AI Assistant Skill Pack for Requirements and Elicitation

## What is it?
`business-analysis-skills` is a platform-neutral library of 53 reusable skills for AI coding/analysis assistants (Claude Code, Codex, and similar agent platforms), covering requirements discovery, elicitation, stakeholder analysis, process work, prioritization, and quality review. It packages each technique as a standalone `SKILL.md` file with YAML frontmatter plus instructions, grouped into atomic techniques, end-to-end workflows, and quality passes, and ships with sync tooling so the same skills can be installed into `.claude/skills/` or `.agents/skills/` in any repo.

## Why it matters for Business Analysts
This repo turns scattered BA know-how (interview techniques, MoSCoW/Kano prioritization, requirements quality checklists, stakeholder mapping) into reusable, agent-callable prompts rather than tribal knowledge locked in someone's head or a static template doc. It lets a BA pair with an AI assistant for first-draft elicitation plans, requirements documents, and quality reviews, then focus human time on judgment calls and stakeholder conversations. Because it's platform-neutral, a BA team isn't locked into one AI vendor's skill format, and the quality-review skills give a repeatable way to catch ambiguous or untestable requirements before they reach development.

## How to use it in BA Workflows
1. **Elicitation prep** - Invoke the elicitation-track skills to generate structured interview guides, workshop agendas, or survey questions tailored to a given stakeholder group before a discovery session.
2. **Requirements drafting** - Use the requirements/specification skills to turn raw notes or transcripts into structured functional/non-functional requirements or user stories in a consistent template.
3. **Stakeholder and process mapping** - Apply the process-work skills to produce RACI matrices, as-is/to-be process outlines, or stakeholder influence/interest grids as a starting draft for review.
4. **Prioritization** - Run the prioritization skills (MoSCoW, Kano, weighted scoring, etc.) against a backlog to get a defensible first-pass ranking the BA can then negotiate with stakeholders.
5. **Quality gate before sign-off** - Pass draft requirements or specs through the quality-review skills to flag ambiguity, missing acceptance criteria, untestable statements, or conflicting requirements before baseline.

## Key Features
- 53 skills organized into 5 tracks spanning atomic techniques, workflows, and quality checks
- Standard `SKILL.md` format (YAML frontmatter + instructions) compatible with Claude's skill-invocation convention
- Dual packaging: canonical source skills plus mirrored copies for `.claude/skills/` and `.agents/skills/`, kept in sync via install/sync scripts
- Includes reusable BA document templates under `docs/ba/templates/`
- Platform-neutral design so the same skill pack works across different agentic AI tools, not just one vendor

## Technology Stack
- **Languages:** Markdown (skill definitions and templates), Shell/Bash and Windows scripts (install/sync tooling)
- **Dependencies:** None beyond a compatible AI agent platform (Claude Code, Codex, or similar) that can load `SKILL.md`-style skills
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Business analysis skill pack for requirements, elicitation, stakeholder analysis, process work, prioritization, and quality checks

## Related Skills
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
