---
date: 2026-09-04
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted, babok, requirements-management, stakeholder-analysis, traceability, mcp, llm]
source: GitHub
---

# AInalyst - AI Business Analyst Assistant for BABOK Workflows

## What is it?
AInalyst is an open-source AI assistant that operationalizes the BABOK v3 (Business Analysis Body of Knowledge) methodology through Claude and the Model Context Protocol (MCP). It packages 21 skills and 114 MCP-based tools covering BABOK chapters 3-7 (Planning, Elicitation, Requirements Lifecycle Management, Analysis, and Design), guiding analysts step by step through structured business analysis activities directly inside VS Code with the Claude Code extension.

## Why it matters for Business Analysts
AInalyst turns a widely-referenced but dense professional standard (BABOK v3) into an executable, AI-guided workflow, making rigorous business analysis practice accessible without years of BABOK study. It benefits experienced analysts looking for efficiency gains on repetitive tasks like impact analysis and traceability, junior BAs who need methodological guardrails while they learn the craft, and product/project managers or small teams who lack a dedicated BA but still need defensible, standards-aligned requirements work. Because it enforces BABOK's nine requirements-quality characteristics and generates artifacts like traceability matrices automatically, it reduces the risk of ambiguous or untestable requirements reaching delivery teams.

## How to use it in BA Workflows
1. **Guided elicitation and interview management** - Use AInalyst's chapter-3/4 tool set to plan stakeholder interviews, capture elicitation results, and structure findings consistently across sessions.
2. **Stakeholder mapping** - Generate stakeholder maps and engagement plans as a first step in any initiative, ensuring influence, interest, and communication needs are documented before requirements work begins.
3. **Requirements quality verification** - Run captured requirements through the tool's BABOK nine-characteristics check (e.g. unambiguous, testable, feasible) to catch weak requirements before they reach a backlog or spec.
4. **Change impact analysis** - When a change request arrives, use the traceability-graph traversal tools to automatically surface every downstream requirement, design element, or test affected by the change.
5. **Prioritization and traceability reporting** - Apply built-in MoSCoW, WSJF, Impact/Effort Matrix, or Time Boxing prioritization methods, then generate traceability matrices and approval-workflow tracking artifacts for governance and audit purposes.

## Key Features
- **BABOK v3 phase coverage** — 21 skills and 114 MCP tools mapped to BABOK chapters 3-7, runnable individually per chapter or as a full methodology suite
- **Automated impact analysis** — Traverses traceability graphs to identify all artifacts affected by a proposed change
- **Multiple prioritization frameworks** — Built-in support for MoSCoW, WSJF, Impact/Effort Matrix, and Time Boxing
- **Requirements quality gate** — Verifies requirements against BABOK's nine quality characteristics before sign-off
- **Methodological guardrails** — Enforces BABOK-aligned process steps rather than freeform AI chat, keeping output consistent and audit-ready

## Technology Stack
- **Languages:** Python 3.10+
- **Dependencies:** Claude Code (VS Code extension), Model Context Protocol (MCP), Anthropic Pro account or higher, Git
- **License:** GNU AGPL v3

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - AI assistant that guides business analysts through BABOK v3 methodology using Claude and MCP tools

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[Stakeholder Analysis Framework]]
- [[OpenFastTrace - Requirements Traceability Suite]]
