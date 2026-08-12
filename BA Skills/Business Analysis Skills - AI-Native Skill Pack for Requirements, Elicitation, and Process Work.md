---
date: 2026-08-12
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, ai-assisted-ba, elicitation, process-modeling]
source: GitHub
---

# Business Analysis Skills - AI-Native Skill Pack for Requirements, Elicitation, and Process Work

## What is it?
Business Analysis Skills is a platform-neutral skill pack of 53 reusable techniques for AI assistants (Claude and other agent frameworks) to perform business analysis work. It bundles atomic BA techniques, end-to-end elicitation workflows, and quality-review passes into a single MIT-licensed repository that installs directly into an agent's skills directory.

## Why it matters for Business Analysts
It turns an AI coding/chat assistant into a structured BA collaborator that follows recognized techniques (PESTLE, SWOT, Porter's Five Forces, RACI, MoSCoW) instead of ad-hoc prompting. Because the skills are organized into discovery, requirements, elicitation, and quality tracks, a BA can ask the assistant to run a specific technique or a full workflow (e.g., stakeholder analysis, process modeling) and get a consistent, standards-aligned deliverable. The quality-check skills (bias assessment, gap review, consistency verification) give BAs a built-in second pass before handing artifacts to stakeholders, reducing rework. Its platform-neutral design means the same skill pack works across Claude and other agent tooling, so teams aren't locked into one AI vendor.

## How to use it in BA Workflows
1. **Business problem framing** - Invoke the workflow skill at project kickoff to structure the problem statement, drivers, and success criteria before requirements work begins.
2. **Stakeholder analysis** - Run the stakeholder-register and power-interest-grid atomic skills to identify, categorize, and prioritize stakeholders for engagement planning.
3. **Elicitation planning** - Use the interview, workshop, and questionnaire design skills to prepare structured elicitation sessions tailored to the audience.
4. **Requirements drafting and review** - Apply acceptance-criteria writing, ambiguity detection, functional/non-functional splitting, and conflict-checking skills to produce clean, testable requirements.
5. **Process and rule capture** - Use as-is/to-be process investigation and business-rule extraction skills to document current-state and future-state processes alongside the rules that govern them.
6. **Pre-delivery quality gate** - Run the deliverable-consistency and evidence-gap-review skills before submitting requirements packages to stakeholders or engineering.

## Key Features
- 53 skills across 5 tracks: atomic techniques, requirements & specification, elicitation extensions, workflows, and quality checks
- Covers classic BA frameworks: PESTLE, SWOT, Porter's Five Forces, RACI/RASCI, MoSCoW prioritization
- End-to-end workflow skills for business problem framing, strategy analysis, stakeholder analysis, requirements elicitation, process modeling, and Soft Systems Methodology
- Quality-assurance skills for bias detection, assumption logging, and deliverable consistency review
- One-command install/uninstall scripts that deploy skills to both `.claude/skills/` and `.agents/skills/` for cross-platform use

## Technology Stack
- **Languages:** Markdown (skill definitions), Bash (install/uninstall scripts)
- **Dependencies:** None — self-contained, platform-neutral skill pack
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Business analysis skill pack for requirements, elicitation, stakeholder analysis, process work, prioritization, and quality checks

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[PM Tools Templates - Comprehensive BA Template Library]]
