---
date: 2026-09-11
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-elicitation, stakeholder-analysis, process-modeling, claude-skills]
source: GitHub
---

# Business Analysis Skills - AI Assistant Skill Pack for BA Methodology

## What is it?
`business-analysis-skills` is a platform-neutral collection of 53 reusable skills that teach AI assistants (Claude Code, Claude Cowork, Claude.ai, and other agentic tools) how to perform structured business analysis work. Instead of a standalone application, it packages BA techniques, requirements-discovery workflows, and quality-review checklists as installable skill files that an AI assistant can invoke on demand.

## Why it matters for Business Analysts
This repo turns an AI assistant into a BA methodology coach and doer: it encodes standard techniques (PESTLE, SWOT, Porter's Five Forces, RACI/RASCI) alongside requirements-engineering discipline (ambiguity detection, constraint identification, gap auditing, conflict checking) so analysts get consistent, repeatable outputs instead of ad-hoc prompting. Because the skills are organized into atomic techniques, end-to-end workflows, and quality checks, a BA can either pull a single technique into a working session or run a full elicitation-to-specification pipeline. It's a practical example of "AI-assisted BA workflows" — the kind of tooling that lets a single analyst scale coverage across discovery, documentation, and review without sacrificing rigor.

## How to use it in BA Workflows
1. **Structured discovery sessions** - Invoke atomic technique skills (PESTLE, SWOT, Porter's Five Forces) during strategy or environment-scanning exercises to get a consistent analytical framework instead of freeform notes.
2. **Stakeholder mapping and RACI/RASCI generation** - Use the stakeholder-mapping and RASCI-building skills to quickly produce accountability matrices from a list of stakeholders and activities.
3. **Requirements quality gating** - Run the ambiguity-detection, constraint-identification, and conflict-checking skills against draft requirements before they go to review, catching issues earlier than a manual read-through.
4. **End-to-end elicitation workflows** - Chain the "workflows" category (problem framing, requirements elicitation, process modeling, requirements packaging) to move from a vague business problem to a packaged requirements artifact in one guided session.
5. **Deliverable quality review** - Apply the quality-check skills (bias review, assumptions logging, evidence-gap analysis, consistency validation) as a final pass before handing off specs or business cases to stakeholders.

## Key Features
- 53 skills across 5 categories: atomic techniques, requirements & specification, elicitation & process extensions, workflows, and quality checks
- Works with any agentic AI assistant that supports the Claude-style skills convention (`.claude/skills/`, `.agents/skills/`)
- Global or per-project installation via `install.sh` / `uninstall.sh` scripts
- Skills are plain-text/markdown definitions, making them easy to read, customize, or extend for an organization's own BA standards
- Companion skill packs referenced by the same maintainer extend into architecture, testing, security, and operations doctrine for teams that want consistent AI-assisted practices across the SDLC

## Technology Stack
- **Languages:** Markdown/plain-text skill definitions, Bash (install/uninstall scripts)
- **Dependencies:** An AI coding assistant that supports the skills convention (e.g., Claude Code, Claude Cowork, Claude.ai)
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Business analysis skill pack for requirements, elicitation, stakeholder analysis, process work, prioritization, and quality checks

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[PM Tools Templates - Comprehensive BA Template Library]]
