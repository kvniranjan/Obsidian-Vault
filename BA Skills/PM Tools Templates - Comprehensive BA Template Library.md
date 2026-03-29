---
date: 2026-03-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, templates, requirements, agile, waterfall, stakeholder-management, risk-management, ai-tools]
source: GitHub
---

# PM Tools Templates - Comprehensive BA Template Library

## What is it?
An open-source collection of 154+ project management and business analysis templates organized by methodology (Traditional, Agile, Hybrid, Universal) and lifecycle phase. Includes a **Requirements Structuring CLI** (v1.1.0) that uses LLMs to convert natural language requirements into formal Use Case Specifications, test cases, and Gherkin/BDD feature files — with built-in ambiguity detection.

Repository: [mirichard/pm-tools-templates](https://github.com/mirichard/pm-tools-templates)

## Why it matters for Business Analysts
BAs constantly need to produce consistent, professional deliverables across different projects and clients. This library provides:
- Ready-to-use templates that save time on formatting and structure
- Coverage across the full BA lifecycle — from requirements elicitation to closure
- An AI-powered CLI that transforms rough, natural-language requirements into properly structured use cases before development begins, catching ambiguity early
- Stakeholder-ready artifacts that communicate clearly across technical and non-technical audiences

## How to use it in BA Workflows

### 1. Pick Templates by Phase
Templates are organized by lifecycle phase:
- **Initiation**: Project charter, stakeholder register, business case
- **Planning**: Requirements traceability matrix, risk register, communication plan
- **Execution**: Change request forms, sprint planning templates, UAT scripts
- **Closure**: Lessons learned, transition plan, handoff documentation

### 2. Use the Requirements Structuring CLI
Convert informal requirements into structured artefacts:
```bash
# Install and run (Python-based)
pip install -r requirements.txt
python req_structurer.py --input "user_stories.txt" --output-format use-case
```
The CLI outputs:
- Formal Use Case Specifications (actor, preconditions, main flow, alternatives)
- Test cases aligned to each requirement
- Gherkin `.feature` files for BDD frameworks like Cucumber

### 3. Ambiguity Detection
Before handing requirements to engineering, run the ambiguity checker to flag:
- Vague terms ("fast", "easy", "secure" without criteria)
- Undefined references (e.g., "the system" without specifying which)
- Missing acceptance criteria

### 4. Adapt to Your Toolchain
Templates are vendor-agnostic — export or adapt for Jira, Confluence, GitHub Issues, Asana, or Microsoft Project.

## Key Features
- 154+ templates across Traditional, Agile, Hybrid, and Universal methodologies
- Requirements Structuring CLI with LLM integration for natural-language → formal spec conversion
- Ambiguity detection before engineering handoff
- 126+ risk management artifacts, 116+ stakeholder management tools
- Industry specializations: healthcare, fintech, manufacturing, construction
- MIT licensed — commercially usable
- Active repo: 1,323+ commits, regularly maintained

## GitHub Resources
- [mirichard/pm-tools-templates](https://github.com/mirichard/pm-tools-templates) — Full template library + Requirements Structuring CLI

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Stakeholder Analysis Framework]]
- [[Thunderdome - Agile Planning and Retro Suite]]
- [[BPMN Assistant (LLM-Powered)]]
