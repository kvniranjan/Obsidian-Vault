---
date: 2026-10-12
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, ai-assisted-ba, prd, traceability, mcp, github]
source: GitHub
---

# MCP GitHub Project Manager - AI-Powered Requirements Traceability and PRD Automation

## What is it?
MCP GitHub Project Manager is a Model Context Protocol (MCP) server that turns GitHub Projects v2, issues, and comments into a full project-management backend for both AI agents and human teams. It exposes a compound tool API (20 tools covering 169 actions) that AI assistants such as Claude Code can call directly to generate PRDs, break them into tasks, and manage the resulting GitHub issues and milestones — with no external database required.

## Why it matters for Business Analysts
The project formalizes the idea-to-delivery pipeline (idea → PRD → use cases → tasks → GitHub issues → milestones → sprints) that BAs are often responsible for stitching together manually across documents, spreadsheets, and ticketing tools. Its traceability-matrix and gap-analysis tools directly support core BA deliverables: linking business requirements to features and use cases, flagging orphaned or unimplemented requirements, and assessing the downstream impact of a requirements change. Because it runs as an MCP server, a BA working inside Claude or another MCP-compatible assistant can generate and refine requirements artifacts conversationally while keeping everything synced to the engineering team's actual GitHub backlog.

## How to use it in BA Workflows
1. **PRD generation from a business idea** - Describe a project objective and success metrics in natural language; the server drafts a structured PRD, which the BA then reviews and refines with stakeholders.
2. **Requirements extraction and traceability** - Automatically pull business requirements from PRD objectives, then build a traceability matrix linking each requirement to the features, use cases, and tasks that implement it.
3. **Use case generation** - Generate actor-goal-scenario use cases (including alternative flows) directly from PRD content, giving BAs a starting draft instead of a blank page.
4. **Gap and coverage analysis** - Run coverage analysis to detect requirements with no linked implementation (orphaned requirements) before a release, and use change-impact analysis when a requirement is modified mid-project.
5. **PRD-to-backlog handoff** - Parse an approved PRD into tasks, complexity estimates, and sprint plans, then push them straight into GitHub Issues and Projects so the backlog stays traceable back to the original requirement.

## Key Features
- Compound tool API: 20 tools exposing 169 discrete actions via a `discover_tools` meta-tool for runtime exploration
- AI-powered PM tools: PRD generation, PRD enhancement via gap analysis, PRD-to-task parsing, complexity analysis, sprint planning, and issue triage
- Traceability matrix: links business requirements → features → use cases → tasks, with orphaned-task detection and change-impact analysis
- Agent orchestration: task checkout, heartbeats, token budgets, and subagent hierarchies for multi-agent delivery teams
- Multi-provider AI support: Anthropic, OpenAI, Google Gemini, Perplexity, or any OpenAI-compatible endpoint; AI keys are optional since core tools work without them
- Full GitHub coverage: Projects v2, issues, pull requests, milestones, releases, actions, and branch protection

## Technology Stack
- **Languages:** TypeScript (Node.js)
- **Dependencies:** MCP SDK, Zod v4, Vercel AI SDK v7, Octokit (`@octokit/rest`), GraphQL, Vitest, Jest, Biome, Docker
- **License:** MIT

## GitHub Resources
- [kunwarVivek/mcp-github-project-manager](https://github.com/kunwarVivek/mcp-github-project-manager) - MCP server using GitHub Projects v2 as an AI-driven PRD, requirements-traceability, and task-management backend

## Related Skills
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[OpenSpec - AI-Powered Spec-Driven Development Framework]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
