---
date: 2026-07-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, requirements-as-code, ai-assisted, decision-management, product-management, mcp, traceability]
source: GitHub
---

# Lore RAC-Core — Requirements as Code for AI-Assisted BA Workflows

## What is it?
RAC-Core (Requirements as Code) is a CLI tool and MCP server that stores your team's requirements, decisions, designs, roadmaps, and prompts as typed Markdown in your repository. It then serves that knowledge read-only to AI coding agents (Claude Code, Cursor, Claude Desktop) so agents cite your documented decisions instead of violating or re-litigating them. Unlike RAG-based approaches, retrieval is fully deterministic — no embeddings, no model calls to decide relevance.

## Why it matters for Business Analysts
BAs are the primary authors of the product knowledge that RAC-Core encodes: requirements, decisions, stakeholder constraints, and design rationale. By storing these artefacts as version-controlled Markdown with typed schemas and CI-validated links, RAC-Core makes BA outputs machine-readable by AI agents across the entire SDLC. This closes the gap between what BAs document and what developers (and their AI tools) actually use, dramatically reducing requirements drift. The HTML portal export lets non-technical stakeholders browse the full requirement corpus with search and citation without any backend service, bridging the gap between technical and business audiences.

## How to use it in BA Workflows
1. **Requirements Authoring** - Write requirements as typed Markdown artefacts with frontmatter schemas; `rac validate` and `rac gate` run in CI to reject malformed requirements, broken links, or references to superseded decisions before they land.
2. **Decision Log Management** - Record architectural and product decisions (ADRs) as first-class artefacts; `rac coverage` flags unapplied decisions and `rac review` surfaces stale items based on configurable age thresholds so nothing silently expires.
3. **AI Agent Grounding** - Connect RAC-Core as an MCP server to Claude Code or Cursor so AI coding agents query the BA's requirement corpus before generating code — agents cite your decisions instead of inventing contradictory ones.
4. **Stakeholder Reporting** - Export the full requirements corpus to a self-contained HTML portal with search and citation for non-technical stakeholders, or push to JSONL for downstream memory stores and graph-based visualizations.
5. **Requirements Health Monitoring** - Use `rac doctor` to surface orphaned artefacts and coverage gaps across requirements, decisions, and designs — giving BAs a continuous traceability health dashboard without a separate tool.

## Key Features
- **Typed Markdown artefacts** — every requirement, decision, or design lives as plain Markdown with a per-type schema validated at write time
- **Deterministic retrieval** — no RAG, no embeddings; agents get exactly the relevant artefacts without hallucination risk in the retrieval layer
- **MCP server integration** — native support for Claude Code, Cursor, and Claude Desktop as AI agent consumers
- **`rac gate` CI enforcement** — blocks broken links, ambiguous references, and superseded decisions from entering the corpus
- **`rac coverage`** — flags unscheduled requirements and unapplied decisions to keep the BA backlog honest
- **`rac doctor`** — corpus health check surfacing orphaned artefacts and structural gaps
- **HTML portal export** — stakeholder-friendly browsable knowledge base requiring no backend service
- **Privacy-first** — no internal LLM calls, no network egress except an opt-in, consent-gated usage ping

## Technology Stack
- **Languages:** Python
- **Dependencies:** MCP (Model Context Protocol) for AI agent connectivity; CLI-only, no server infrastructure required
- **License:** Check repository for current license

## GitHub Resources
- [itsthelore/rac-core](https://github.com/itsthelore/rac-core) - Requirements as Code CLI and MCP server for grounding AI agents in team product decisions

## Related Skills
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[OSRMT - Open Source Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
