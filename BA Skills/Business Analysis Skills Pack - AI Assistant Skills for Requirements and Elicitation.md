---
date: 2026-09-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-management, stakeholder-analysis, elicitation, claude-skills]
source: GitHub
---

# Business Analysis Skills Pack - Platform-Neutral BA Skill Pack for AI Assistants

## What is it?
Business Analysis Skills is an open-source collection of 53 reusable business-analysis techniques packaged as skills for AI assistants like Claude and other agent platforms. It bundles atomic BA techniques, requirements and specification helpers, elicitation extensions, end-to-end workflows, and quality-review passes into a single installable pack, mirrored into both `.claude/skills/` and `.agents/skills/` directories.

## Why it matters for Business Analysts
It turns an AI assistant into a structured BA co-pilot rather than a generic chatbot, giving it named, repeatable techniques (PESTLE, SWOT, RACI, MoSCoW, CATWOE) instead of ad-hoc prompting. Because the skills are platform-neutral markdown files, a BA can standardize how their whole team elicits, drafts, and quality-checks requirements regardless of which AI tool colleagues use. The quality-check category is particularly valuable, since it separates deliverable drafting from bias and consistency review, encouraging analysts to critique AI-assisted output before handoff. It's a lightweight way to bring AI-assisted BA workflows into daily practice without adopting a full platform.

## How to use it in BA Workflows
1. **Strategic framing** - Run the Business Problem Framing and Strategy Analysis workflow skills (PESTLE, SWOT Prioritization, Porter's Five Forces, Value Proposition Analysis) at project kickoff to ground requirements work in business context.
2. **Stakeholder analysis** - Use the Stakeholder Register, Power-Interest Grid, and RACI/RASCI Builder skills to identify stakeholders, map influence, and clarify decision rights before elicitation begins.
3. **Elicitation planning and execution** - Apply Interview Design, Questionnaire Design, Workshop Design, and the Pyramid-Funnel-Diamond Interviewer skill to structure elicitation sessions, then use Probe Question Generator for follow-up depth.
4. **Requirements drafting and hardening** - Feed raw notes through Proto-Requirements Normalizer, Ambiguity Hunter, Assumption Extractor, Constraint Detector, and Acceptance Criteria Writer to turn loose statements into testable requirements.
5. **Quality assurance before handoff** - Run the Requirements Quality Check, Requirements Gap Auditor, Requirements Conflict Checker, and Critical Thinking Bias Check skills as a final gate, then use the Requirements Packager workflow to assemble the deliverable.

## Key Features
- 53 individually invokable skills spanning atomic techniques, requirements/specification, elicitation extensions, workflows, and quality checks
- Platform-neutral packaging installed into both `.claude/skills/` and `.agents/skills/` for cross-tool compatibility
- Global or project-level installation via simple `install.sh`/`uninstall.sh` scripts
- Dedicated quality-check category (bias detection, evidence-gap review, deliverable consistency) separate from drafting skills
- Reusable BA templates included under `docs/ba/templates/`
- Covers the full BA lifecycle from strategy framing through elicitation, specification, and packaging

## Technology Stack
- **Languages:** Markdown (SKILL.md definitions), Bash (install/uninstall scripts)
- **Dependencies:** Bash shell environment; no external runtime or language dependencies
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Business analysis skill pack for requirements, elicitation, stakeholder analysis, process work, prioritization, and quality checks

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
