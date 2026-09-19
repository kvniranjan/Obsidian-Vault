---
date: 2026-09-19
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-ba, babok, requirements-management, stakeholder-analysis, decision-management, mcp]
source: GitHub
---

# AInalyst - AI-Powered BABOK v3 Business Analysis Platform

## What is it?
AInalyst is an open-source AI assistant built on Claude and Claude Code that helps business analysts work through the BABOK v3 (IIBA) methodology. It layers 21 skills across 22 MCP servers (114 tools) on top of Claude Code so it can read project files, run analysis, and generate artifacts automatically, acting like a "seasoned analyst colleague" for requirements, prioritization, and stakeholder work.

## Why it matters for Business Analysts
AInalyst directly targets the repetitive, judgment-heavy parts of the BA role: turning interview transcripts into structured requirements, tracing the ripple effects of a change request across a project's artifacts, and validating requirements against BABOK's nine quality characteristics. Because it encodes BABOK chapters 3-7 as reusable skills, it lets junior analysts or non-specialist PMs produce enterprise-grade deliverables without years of BABOK training, while experienced analysts can offload the mechanical documentation work. Its graph-based impact analysis and multi-methodology prioritization (MoSCoW, WSJF, Impact/Effort) make it especially useful on long, multi-month engagements where keeping artifacts consistent by hand becomes error-prone.

## How to use it in BA Workflows
1. **Requirements Elicitation from Interviews** - Feed interview transcripts (.txt, .md, .pdf, .docx) to AInalyst to automatically extract candidate requirements, risks, and stakeholder concerns instead of manually re-reading notes.
2. **Requirements Quality Review** - Run generated or existing requirements through AInalyst's validator, which checks each one against BABOK's nine requirement quality characteristics (e.g. unambiguous, verifiable, feasible) before they go to stakeholders.
3. **Change Impact Analysis** - Use the graph-traversal impact analysis to see which requirements, stakeholder maps, and traceability entries are affected before approving a change request, reducing missed downstream effects.
4. **Requirement and Backlog Prioritization** - Apply the built-in MoSCoW, WSJF, or Impact/Effort methods to prioritize a backlog in a way appropriate to the project's context (regulatory, agile, or startup).
5. **Governance Artifact Generation** - Auto-generate stakeholder maps, traceability matrices, and prioritization documents as Markdown, with optional publishing to Confluence for team visibility.

## Key Features
- 21 domain skills covering BABOK Knowledge Areas (chapters 3-7) surfaced through semantic triggers matched to user requests
- 22 MCP servers exposing 114 tools for requirements analysis, stakeholder mapping, and prioritization
- Graph-based change impact analysis across interconnected project artifacts
- Multi-format interview/document ingestion (.txt, .md, .pdf, .docx)
- Nine-characteristic BABOK requirements quality validation
- Versioned artifact history stored locally (`.history/`) plus optional Confluence sync

## Technology Stack
- **Languages:** Python
- **Dependencies:** Claude Code (VS Code extension), Anthropic Claude, Model Context Protocol (MCP) servers, Anthropic Pro account
- **License:** GNU AGPLv3 (commercial license available for closed-source/SaaS use)

## GitHub Resources
- [chaussky/ainalyst](https://github.com/chaussky/ainalyst) - Open-source Claude/MCP-based AI assistant implementing BABOK v3 for business analysts

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[Stakeholder Analysis Framework]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
