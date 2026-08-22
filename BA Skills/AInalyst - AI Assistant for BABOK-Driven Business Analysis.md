---
date: 2026-08-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, requirements-engineering, babok, claude-code, mcp]
source: GitHub
---

# AInalyst - AI Assistant for BABOK-Driven Business Analysis

## What is it?
AInalyst is an open-source AI assistant that guides business analysts through the BABOK v3 methodology directly inside VS Code via Claude Code. It acts as an intelligent colleague across the full BA lifecycle — planning, elicitation, traceability, analysis, and design — proposing next steps conversationally while handling the technical execution of artifact creation, tracing, and validation behind the scenes.

## Why it matters for Business Analysts
Most AI coding assistants are built for developers, not BAs — AInalyst is purpose-built around the BABOK body of knowledge, so its prompts, tools, and validations map directly to the vocabulary and deliverables BAs already use (stakeholder maps, elicitation plans, traceability matrices, change impact analysis). It lets a junior analyst perform senior-level requirement quality checks against all nine BABOK characteristics, and gives small teams or startups a way to apply professional BA discipline without a dedicated toolchain. Because it's phase-aware, it only loads the tools relevant to the current BABOK chapter, keeping the workflow focused rather than overwhelming.

## How to use it in BA Workflows
1. **Change Impact Analysis** - Describe a change request in chat; AInalyst runs a BFS traversal of the project's traceability graph to surface every affected artifact (requirements, designs, tests) before you commit to scope.
2. **Requirement Prioritization** - Apply MoSCoW, WSJF, Impact/Effort, or Time Boxing methods conversationally to rank competing requirements for a release.
3. **Elicitation Support** - Use the Chapter 4 toolset during interviews and workshops to capture transcripts and convert them into structured elicitation artifacts.
4. **Quality Verification** - Validate draft requirements against BABOK's nine quality characteristics (e.g., unambiguous, verifiable, feasible) before handing them to development.
5. **Artifact Publishing** - Generate governance plans, specifications, and reports as versioned Markdown and publish them directly to Confluence for stakeholder review.

## Key Features
- 21 skills and 22 MCP servers (114 tools total) organized by BABOK chapter (Planning, Elicitation, Lifecycle Management, Analysis, Design)
- Phase-based tool loading keeps the assistant focused on the current stage of the BA lifecycle
- Traceability graph with BFS-based impact analysis across 11+ artifact types
- Four built-in prioritization frameworks (MoSCoW, WSJF, Impact/Effort, Time Boxing)
- Version-controlled artifacts (Markdown/JSON) with automatic `.history/` snapshots
- Confluence publishing integration

## Technology Stack
- **Languages:** Python 3.10+
- **Dependencies:** Claude Code (Anthropic), Model Context Protocol (MCP) servers, VS Code extension host
- **License:** GNU AGPL v3 (open-source); commercial licenses available for SaaS/closed-source use

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - AI assistant guiding business analysts through BABOK v3 via Claude Code and MCP

## Related Skills
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
