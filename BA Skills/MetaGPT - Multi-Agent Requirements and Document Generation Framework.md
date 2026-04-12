---
date: 2026-04-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, multi-agent, requirements, PRD, user-stories, document-generation, LLM, AI-agent]
source: GitHub
---

# MetaGPT - Multi-Agent Requirements and Document Generation Framework

## What is it?
[MetaGPT](https://github.com/FoundationAgents/MetaGPT) is an open-source multi-agent framework with 57,500+ GitHub stars that simulates a full software company — with AI agents acting as product managers, architects, engineers, and project managers — to turn a single natural-language requirement into complete deliverables including PRDs, user stories, competitive analysis, system designs, and code. Developed by DeepWisdom and now maintained under the FoundationAgents organization, MetaGPT orchestrates specialized agents using Standard Operating Procedures (SOPs) to produce structured, professional-grade output. In early 2025, the team launched MGX (MetaGPT X), billed as the world's first AI agent development team, and their AFlow workflow paper was accepted for oral presentation (top 1.8%) at ICLR 2025.

## Why it matters for Business Analysts
Business analysts spend a significant portion of their time converting stakeholder conversations into structured documents — PRDs, BRDs, FRS, user stories — a tedious and error-prone process. MetaGPT can take a single-sentence requirement and generate a multi-section PRD including user stories, competitive analysis, and requirement breakdowns within minutes, dramatically compressing the elicitation-to-documentation cycle. The framework's role-based agent architecture mirrors how BA teams actually work, making outputs familiar and easy to review. Because it runs locally or against any supported LLM, sensitive project requirements can remain within organizational boundaries. For BAs tasked with requirements validation, MetaGPT's architectural and data-structure outputs can also help rapidly cross-check feasibility with technical counterparts.

## How to use it in BA Workflows
1. **PRD Generation from Stakeholder Input** — Feed a one-sentence business need (e.g., "Build a customer loyalty portal for retail banking") and receive a complete Product Requirements Document with goals, user stories, competitive landscape, and prioritized requirements list.
2. **User Story Factory** — Use the Product Manager agent in isolation to rapidly generate and expand user story backlogs from high-level epics, saving days of manual decomposition.
3. **Competitive Analysis Automation** — Trigger MetaGPT's competitive analysis module to benchmark a proposed product against market alternatives and surface differentiators for stakeholder presentations.
4. **Gap Analysis Support** — Provide existing system documentation and a new capability requirement; MetaGPT agents can identify missing features and produce a structured gap report.
5. **Feasibility Pre-Assessment** — Let the Architect agent review requirements and output a high-level system design, giving BAs an early technical sanity check before formal design workshops begin.

## Key Features
- Single-prompt to full documentation pipeline (PRD, user stories, design, tasks, code)
- Specialized role-based agents: Product Manager, Architect, Project Manager, Engineer
- Standardized Operating Procedures (SOPs) for consistent, repeatable output quality
- Multi-LLM support: GPT-4, Claude, open-source models (Ollama, DeepSeek)
- Agentic workflow automation via AFlow for customizable pipeline generation
- Structured JSON/Markdown output compatible with Obsidian and Confluence imports
- Extensible — custom roles and actions can be added for domain-specific BA tasks
- Active research backing: ICLR 2025 paper, 57,500+ stars, continuous releases

## Technology Stack
- **Languages:** Python
- **LLM Support:** OpenAI GPT-4/GPT-4o, Anthropic Claude, Ollama (local), DeepSeek, Azure OpenAI
- **Dependencies:** pydantic, aiohttp, openai SDK, anthropic SDK, tiktoken, tenacity, rich

## GitHub Resources
- [FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) — Multi-agent framework that converts a one-line requirement into PRD, design, user stories, and code

## Related Skills
- [[CrewAI - Role-Based Multi-Agent Orchestration Framework]]
- [[LangGraph - AI Agent Orchestration Framework]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
