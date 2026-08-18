---
date: 2026-08-18
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements, elicitation, stakeholder-analysis, process-modeling]
source: GitHub
---

# Business Analysis Skills - AI Assistant Skill Pack for Requirements, Elicitation, and Process Work

## What is it?
Business Analysis Skills is a platform-neutral collection of 53 Markdown-based skill definitions designed to teach AI assistants how to perform structured business analysis work. It packages atomic techniques (PESTLE, SWOT, Porter's Five Forces, stakeholder mapping, RACI), requirements and specification skills, elicitation support, end-to-end workflows, and quality review passes into one reusable repository that can be installed globally or copied into individual projects.

## Why it matters for Business Analysts
This repository turns an AI assistant into a structured BA co-pilot rather than a generic chatbot, guiding it through the same discovery, elicitation, specification, and quality-check disciplines a trained analyst would follow. It codifies techniques that are often scattered across BABOK references and training materials (PESTLE, SWOT prioritization, stakeholder communication planning, ambiguity detection, conflict checking) into consistent, repeatable prompts. For BAs already using AI tools for drafting requirements or facilitating workshops, it provides a vetted, technique-grounded scaffold instead of ad-hoc prompting, reducing the risk of missing steps like bias checking or evidence-gap review before handing off a deliverable.

## How to use it in BA Workflows
1. **Problem Framing & Strategy Analysis** - Use the workflow skills to structure early-stage discovery, running PESTLE or Porter's Five Forces analyses with the AI assistant before requirements work begins.
2. **Stakeholder Analysis & Communication Planning** - Apply the stakeholder mapping and RACI matrix skills to identify stakeholders, assign responsibilities, and generate a tailored communication plan.
3. **Requirements Elicitation & Specification** - Run interview/workshop design skills to prepare elicitation sessions, then use the specification skills to draft and refine acceptance criteria.
4. **Process Investigation & Business Rule Extraction** - Use the elicitation and process extension skills to document as-is processes and extract business rules from stakeholder input or existing documentation.
5. **Quality Review Before Handoff** - Run the quality-check skills (ambiguity detection, gap auditing, conflict checking, bias checking) on drafted requirements before delivering them to development or product teams.

## Key Features
- 53 skills organized across 5 tracks: atomic techniques, requirements & specification, elicitation & process extensions, workflows, and quality checks
- Platform-neutral design that works with any AI assistant supporting Markdown-based skill/prompt loading
- Global install script or per-project copy option for flexible adoption
- Built-in quality gates (bias checking, evidence gap review, consistency validation) to catch issues before deliverable handoff
- Covers classic BA frameworks (PESTLE, SWOT, Porter's Five Forces, RACI) alongside modern requirements-quality techniques (ambiguity and conflict detection)

## Technology Stack
- **Languages:** Markdown (skill/prompt definitions), Bash (install script)
- **Dependencies:** None beyond an AI assistant capable of loading Markdown-based skills
- **License:** MIT

## GitHub Resources
- [45ck/business-analysis-skills](https://github.com/45ck/business-analysis-skills) - Platform-neutral business analysis skill pack for AI assistants covering elicitation, requirements, and quality review workflows

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Stakeholder Analysis Framework]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[PM Tools Templates - Comprehensive BA Template Library]]
