---
date: 2026-09-01
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-engineering, ai-assisted, babok, stakeholder-analysis, traceability, ai-ba-workflows]
source: GitHub
---

# AInalyst - AI Assistant for BABOK-Aligned Business Analysis

## What is it?
AInalyst is an open-source, AI-powered assistant built on the Claude Code agent framework that helps business analysts work through projects in line with the BABOK v3 (Business Analysis Body of Knowledge) methodology. It functions as a conversational "seasoned analyst colleague," combining 21 skills and 22 MCP (Model Context Protocol) servers exposing 114 tools that cover BABOK chapters 3 through 7.

## Why it matters for Business Analysts
Most AI coding assistants are built for developers, not analysts — AInalyst is purpose-built around the BA's own body of knowledge, so its prompts, artifacts, and quality checks map directly onto techniques BAs already use (stakeholder maps, elicitation plans, prioritization matrices). It enforces methodology rigor automatically, running quality checks against BABOK's requirement characteristics and flagging ambiguous or non-atomic statements before they reach stakeholders. Because it maintains a structured requirements graph, impact analysis on change requests becomes a traversal rather than a manual re-read of every document. It keeps analysts in the decision-making seat while automating the repetitive documentation and traceability work that consumes a large share of BA time.

## How to use it in BA Workflows
1. **Elicitation and interview support** - Describe an upcoming stakeholder interview conversationally; AInalyst proposes questions, structures the session, and generates interview minutes as a tracked artifact afterward.
2. **Stakeholder mapping** - Build and maintain stakeholder maps that update as new stakeholders and relationships are discovered during discovery activities.
3. **Requirement prioritization** - Apply MoSCoW, Weighted Shortest Job First (WSJF), an Impact/Effort Matrix, or Time Boxing, letting the assistant recommend the methodology best suited to the current project context.
4. **Requirement quality verification** - Validate draft requirements against BABOK's nine quality characteristics, catching ambiguity, missing acceptance criteria, and non-atomic statements before sprint planning.
5. **Impact analysis and traceability** - When a change request arrives, traverse the requirements graph automatically to identify every downstream artifact, specification, and stakeholder affected.

## Key Features
- 21 conversational skills and 22 MCP servers (114 tools) covering BABOK chapters 3-7
- Semantic trigger matching activates the right skill from natural-language requests
- Structured, versioned artifact generation (BA plans, stakeholder maps, interview minutes, specifications) in Markdown
- Built-in requirement quality gate against BABOK's nine requirement characteristics
- Optional multi-agent task splitting to separate reasoning from artifact generation on large projects
- Optional Confluence integration for publishing finished artifacts

## Technology Stack
- **Languages:** Python 3.10+
- **Dependencies:** Claude Code agent framework (VS Code extension), Model Context Protocol (MCP) servers, optional Confluence API integration
- **License:** GNU AGPL v3 (commercial licensing available)

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - AI assistant that helps business analysts work to the BABOK v3 methodology

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
- [[OSRMT - Open Source Requirements Management Tool]]
