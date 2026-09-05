---
date: 2026-09-05
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted, babok, requirements-engineering, stakeholder-analysis, mcp, ai-agent]
source: GitHub
---

# AInalyst - AI Agent Platform for BABOK-Driven Business Analysis

## What is it?
AInalyst is an AI-powered assistant built on Claude that helps business analysts (or anyone acting as one on a project) work through the BABOK v3 methodology end-to-end. It ships as a set of skills and MCP servers exposing over a hundred tools that cover BABOK chapters 3 through 7, handling stakeholder interviews, requirements elicitation, traceability, and artifact generation directly inside an agentic workflow.

## Why it matters for Business Analysts
AInalyst operationalizes BABOK rather than just referencing it — it turns the standard's knowledge areas (Planning & Monitoring, Elicitation & Collaboration, Requirements Life Cycle Management, Strategy Analysis, and Requirements Analysis & Design Definition) into callable tools an AI agent can execute during real BA work. This lets analysts offload repetitive artifact drafting (stakeholder maps, requirements specs, traceability matrices) while keeping outputs structured and standards-aligned. Built-in support for multiple prioritization frameworks (MoSCoW, WSJF, Impact/Effort) and Confluence publishing means the tool fits directly into existing BA deliverable pipelines instead of requiring a parallel process. For BAs already using Claude Code or other MCP-compatible agents, it is a drop-in methodology layer rather than a separate application to learn.

## How to use it in BA Workflows
1. **Stakeholder Analysis** - Feed interview transcripts or meeting notes to AInalyst's elicitation tools to auto-generate stakeholder maps and RACI-style breakdowns aligned with BABOK's Elicitation & Collaboration knowledge area.
2. **Requirements Elicitation & Documentation** - Process raw inputs (transcripts, regulations, existing specs) into structured requirements artifacts, reducing manual transcription and formatting work during discovery.
3. **Requirements Traceability** - Generate and maintain traceability matrices automatically as requirements evolve, so links between business needs, requirements, and solution components stay current without manual spreadsheet upkeep.
4. **Prioritization & Planning** - Apply MoSCoW, WSJF, or Impact/Effort matrices to a backlog of requirements to produce a defensible, methodology-grounded prioritization output for stakeholder review.
5. **Artifact Publishing** - Push finished plans, specifications, and stakeholder maps directly to Confluence, keeping the BA's documentation of record in sync with the tool's output without manual copy-paste.

## Key Features
- **21 skills and 22 MCP servers with 114 tools** spanning BABOK chapters 3-7 for planning, elicitation, traceability, and analysis
- **Phase-based tool loading** — loads only the MCP tools relevant to the current task to keep agent context usage efficient
- **Multi-agent task splitting** — complex requests are decomposed across specialized agents for dialogue, task breakdown, reasoning, and artifact writing
- **Multiple prioritization methodologies** built in (MoSCoW, WSJF, Impact/Effort Matrix)
- **Confluence integration** for direct publishing of generated artifacts
- **Input file processing** for transcripts, regulatory text, and existing specification documents

## Technology Stack
- **Languages:** Python
- **Dependencies:** MCP (Model Context Protocol) servers; Claude/Claude Code as the underlying agent runtime
- **License:** AGPL-3.0 (commercial licensing option also available)

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - AI agent platform implementing BABOK v3 methodology for business analysts via Claude and MCP

## Related Skills
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Stakeholder Analysis Framework]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
