---
date: 2026-08-30
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-management, stakeholder-analysis, elicitation, process-modeling]
source: GitHub
---

# Business Analysis Skills - Platform-Neutral AI Skill Pack for BA Work

## What is it?
Business Analysis Skills is an open-source, platform-neutral skill pack that packages 53 discrete business-analysis techniques into reusable "skills" for AI assistants such as Claude. It spans atomic techniques (PESTLE, SWOT, RACI, stakeholder registers), requirements and specification work, elicitation extensions, end-to-end workflows, and quality-review passes, all distributed as Markdown/YAML skill definitions built on the Claude Agent SDK skill format.

## Why it matters for Business Analysts
This repo turns a BA's own body of practice into something an AI assistant can execute consistently and repeatably, rather than relying on ad-hoc prompting. It covers gaps many AI-for-BA tools miss: requirements traceability initialization, ambiguity detection, assumption/constraint extraction, and structured quality checks before handoff. Because skills are organized into discovery → requirements → elicitation → workflow → quality tracks, a BA can invoke exactly the right technique at the right stage of an engagement instead of writing bespoke prompts each time. The included sample use cases (claims triage, payroll replacement, CRM migration, procurement improvement) show it is grounded in real BA deliverables, not generic prompt templates.

## How to use it in BA Workflows
1. **Stakeholder & Strategy Framing** - Use the business-problem-framing and strategy-analysis workflow skills at project kickoff to structure PESTLE, SWOT, and Porter's Five Forces analysis before requirements work begins.
2. **Elicitation Planning** - Apply the elicitation-extension skills (interview design, questionnaire validation, workshop/breakout structuring, probe-question generation) to prepare structured elicitation sessions with stakeholders.
3. **Requirements Drafting & Hardening** - Run the requirements-and-specification skills to write acceptance criteria, separate functional from non-functional requirements, extract assumptions/constraints, and detect ambiguity or conflicts in draft requirements.
4. **Process & Rule Discovery** - Use the as-is/to-be process investigation and business-rule extraction skills to document current-state processes and derive rules for redesign, complementing dedicated BPMN tools.
5. **Quality Assurance Before Handoff** - Apply the quality-check skills (bias review, evidence-gap analysis, deliverable consistency, requirements quality verification) as a final pass before requirements are handed to delivery teams.

## Key Features
- 53 skills across 5 tracks: Atomic Techniques (17), Requirements & Specification (14), Elicitation & Process Extensions (10), Workflows (7), Quality Checks (5)
- Global install (`~/.claude/skills/`, `~/.agents/skills/`) or per-project install via copying `.claude/` and `.agents/` directories
- Dual packaging for both Claude-native and general `.agents/skills/` ecosystems, keeping platform neutrality
- Includes RACI/RASCI builders, MoSCoW prioritization, root-cause analysis, and traceability initialization as ready-to-run skills
- Ships with an uninstall script for clean removal of globally installed skills

## Technology Stack
- **Languages:** Markdown/YAML skill definitions, Bash installer scripts
- **Dependencies:** Anthropic Claude Agent SDK skill format; compatible with `.claude/` and `.agents/` skill directory conventions
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Platform-neutral AI skill pack of 53 business analysis techniques for requirements, elicitation, and quality review

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
