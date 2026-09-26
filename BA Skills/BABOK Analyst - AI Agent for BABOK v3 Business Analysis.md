---
date: 2026-09-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted, babok, iiba, requirements, business-case, roi, mcp, claude-ai]
source: GitHub
---

# BABOK Analyst - AI Agent for BABOK v3 Business Analysis

## What is it?
BABOK Analyst is an open-source, AI-powered system that turns LLMs (Claude, ChatGPT, Gemini, and others) into a professional business analysis agent compliant with the IIBA's BABOK v3 standard. It walks an analyst through a structured 9-stage flow — from a Stage 0 project charter through Stage 8 business case and ROI — with human-in-the-loop approval gates at every stage. It ships as modular system prompts, a Node.js CLI, an MCP server, and a Next.js web UI, so it can run inside Claude Code, Claude Desktop, ChatGPT, or a browser.

## Why it matters for Business Analysts
This is one of the few open-source tools built specifically around the BABOK methodology rather than generic project management or generic LLM chat. It encodes the discipline of a real BA engagement — sponsor sign-off, stakeholder mapping, current-state analysis, root-cause and prioritization, requirements and user stories, target-state design, gap analysis, risk register, and financial modeling — as an enforceable, auditable workflow rather than a one-off prompt. The "Short Rationale + Evidence" methodology and built-in cross-stage consistency checks (requirement traceability, budget ceiling, integration coverage) push analysts toward defensible, evidence-backed deliverables instead of AI-hallucinated boilerplate. Document ingestion (PDF/DOCX/XLSX/CSV) and DOCX/PDF export make it practical to plug into an existing BA engagement's real inputs and outputs.

## How to use it in BA Workflows
1. **Project Chartering** - Run Stage 0 to capture sponsor sign-off, scope boundaries, and a Go/No-Go gate before any analysis work begins, preventing scope creep from day one.
2. **Stakeholder and Current-State Analysis** - Use Stages 1-2 to build stakeholder maps, success criteria, current-state process maps, cost baselines, and system inventories, all captured as versioned Markdown project files.
3. **Requirements Elicitation and Prioritization** - Use Stages 3-4 to categorize problems, run root-cause analysis, and draft functional/non-functional requirements and user stories with MoSCoW prioritization, with automated quality scoring against SMART criteria.
4. **Target-State Design and Roadmapping** - Use Stages 5-6 to define target architecture, future-state process design, and a gap-analysis-driven implementation roadmap that a delivery team can act on directly.
5. **Risk and Business Case Delivery** - Use Stages 7-8 to produce a risk register with mitigations and a financial model (ROI, NPV, payback period), then export the full package as Markdown, DOCX, or PDF for sponsor sign-off.

## Key Features
- 9-stage BABOK v3-aligned workflow with human-in-the-loop approval at each stage
- MCP server (`babok-mcp`) exposing 32 tools and 9 resources for Claude Desktop and other MCP clients
- Node.js CLI (`babok`) for project lifecycle management, interactive stage interviews, and quality scoring
- Next.js web UI for collaborative, browser-based project review and stage interviews
- Advanced model routing with automatic failover across Anthropic, OpenAI, Google Gemini, Hugging Face, and Vertex AI
- Built-in cross-stage consistency validation (requirement traceability, budget ceiling, integration coverage) and automated quality scoring
- Document ingestion (PDF/DOCX/XLSX/CSV/TXT/MD) and export to Markdown, DOCX, and PDF
- File locking for safe concurrent editing on shared/team drives

## Technology Stack
- **Languages:** Node.js/JavaScript, TypeScript, Python (tooling), Markdown (prompts and artefacts)
- **Dependencies:** Model Context Protocol (MCP), Next.js 15, Anthropic/OpenAI/Google Gemini/Hugging Face/Vertex AI SDKs
- **License:** MIT

## GitHub Resources
- [GSkuza/BABOK_ANALYST](https://github.com/GSkuza/BABOK_ANALYST) - AI agent guiding analysts through a 9-stage BABOK v3-compliant business analysis workflow

## Related Skills
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Stakeholder Analysis Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
