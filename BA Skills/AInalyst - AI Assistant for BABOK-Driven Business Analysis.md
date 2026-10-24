---
date: 2026-10-24
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted, babok, requirements-engineering, elicitation, claude-code, mcp]
source: GitHub
---

# AInalyst - AI Assistant for BABOK-Driven Business Analysis

## What is it?
AInalyst is an open-source AI assistant, built to run on Claude through Claude Code, that helps business analysts carry out BABOK v3-aligned work end to end. It packages 21 skills and 22 MCP servers exposing 114 tools covering BABOK chapters 3 through 7 (planning, elicitation, requirements lifecycle management, strategy analysis, and requirements analysis/design), splitting work across dedicated dialogue, planning, reasoning, and writing agents so large analysis tasks stay organised and auditable.

## Why it matters for Business Analysts
Most AI tools help with a single BA artefact; AInalyst instead structures an entire engagement around a recognised body of knowledge, so the outputs map directly to what stakeholders and auditors expect from a BABOK-trained analyst. Its traceability-graph-driven change impact analysis and built-in requirements quality checks (against the nine BABOK characteristics) catch the kind of gaps that normally surface late in a project, while its prioritisation engine (MoSCoW, WSJF, Impact/Effort, time boxing) automates a judgment call analysts make constantly. Because it ingests existing inputs (.txt, .md, .pdf, .docx) and writes deterministic, rerunnable Markdown artefacts — with optional Confluence publishing — it fits into existing documentation workflows rather than replacing them, and it keeps the analyst as the final decision-maker rather than automating judgement away.

## How to use it in BA Workflows
1. **BABOK-aligned discovery engagement** - Point AInalyst at a folder of stakeholder documents and run the `full` phase to produce a complete set of planning, elicitation, and analysis artefacts consistent with BABOK structure, giving a new engagement a standards-based starting point.
2. **Change request impact analysis** - Feed a proposed change into the assistant and have it traverse the requirements traceability graph to surface affected artefacts and conflicts (e.g. a clash with an existing performance requirement) before the change is approved.
3. **Requirements quality gate** - Run draft requirements through the nine-characteristic BABOK quality check to catch ambiguity or untestability early, using the suggested rewordings as a teaching tool for junior analysts.
4. **Prioritisation facilitation** - Let the assistant pick and apply the most suitable prioritisation technique (MoSCoW, WSJF, Impact/Effort matrix, time boxing) for a given backlog or initiative, producing a defensible, repeatable rationale.
5. **Governance documentation and publishing** - Generate governance plans and reports as Markdown artefacts under version control, then publish finalised outputs directly to Confluence for stakeholder visibility without manual reformatting.

## Key Features
- **BABOK v3 chapter coverage** — 21 skills mapped to BABOK chapters 3-7 (planning, elicitation, lifecycle management, strategy, analysis/design)
- **Multi-agent architecture** — Separate dialogue, planning, reasoning, and writing agents, with deterministic writing steps that can be safely rerun on failure
- **Traceability-graph impact analysis** — Automatically identifies affected artefacts and conflicts when a change request is introduced
- **Nine-characteristic requirements quality checks** — Validates requirements against BABOK's own quality criteria and suggests concrete rewordings
- **Automated prioritisation** — Applies MoSCoW, WSJF, Impact/Effort, or time boxing depending on context
- **Flexible input/output** — Ingests .txt/.md/.pdf/.docx inputs and writes Markdown artefacts, with optional Confluence publishing

## Technology Stack
- **Languages:** Python (3.10+)
- **Dependencies:** Claude Code, Anthropic Claude, Model Context Protocol (MCP) servers
- **License:** GNU AGPL v3 (commercial license available for closed-source or hosted use)

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - AI assistant that guides business analysts through BABOK v3-aligned planning, elicitation, and analysis using Claude Code

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
