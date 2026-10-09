---
date: 2026-10-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, genbi, text-to-sql, semantic-layer, ai-assisted-ba-workflows]
source: GitHub
---

# WrenAI - Governed Text-to-SQL and GenBI Engine for AI Agents

## What is it?
WrenAI (Canner/WrenAI) is an open-source GenBI (Generative BI) engine that gives AI agents a governed semantic layer so natural-language business questions turn into validated SQL, dashboards, and charts rather than guessed queries. It works across 20+ data sources (BigQuery, Snowflake, PostgreSQL, ClickHouse, Redshift, Databricks, DuckDB) on top of a single Apache DataFusion-powered engine, and plugs directly into Claude Code, Cursor, Cline, Codex, and other MCP-compatible agents.

## Why it matters for Business Analysts
BAs are regularly asked to turn ad-hoc "what does the data say" questions into trustworthy answers, and the biggest risk in doing this with AI is a model inventing a join or redefining a metric like "revenue" differently each time. WrenAI's Modeling Definition Language (MDL) lets a BA encode approved models, relationships, metrics, and business definitions once, in reviewable YAML/Markdown committed to Git, so every agent-generated answer is checked against the same governed rules. That turns data analysis from a one-off SQL request into a repeatable, auditable workflow, and lets BAs review metric or semantic changes through normal pull requests rather than tribal knowledge. It also lowers the barrier for non-technical stakeholders to self-serve answers without bypassing governance.

## How to use it in BA Workflows
1. **Governed self-service analytics** - Model the business's core entities and metrics once in MDL, then let stakeholders ask natural-language questions through an AI agent and get SQL/dashboards that always respect the agreed definitions.
2. **Metric definition reviews** - Store metric and business-context changes (`instructions.md`, `queries.yml`) in Git so a BA can review proposed definition changes via pull request before they go live, the same way requirements changes are reviewed.
3. **Requirements-to-data validation** - Use `wren ask`/`wren query` to quickly check whether a proposed requirement or KPI is actually derivable from existing data models, surfacing data gaps early in elicitation.
4. **Stakeholder-ready dashboards** - Generate charts and dashboards from business questions and publish them to Vercel/Cloudflare Pages for sharing with stakeholders who need a quick visual rather than a raw answer.
5. **AI-assisted BA workflows** - Wire WrenAI's skills/MCP integration into Claude Code or another agent so a BA's existing AI assistant can answer data questions from live warehouses using the same vetted semantic context used elsewhere in the organization.

## Key Features
- **Governed text-to-SQL** - questions are planned against the semantic layer and dry-run validated before execution, reducing hallucinated joins or columns.
- **Modeling Definition Language (MDL)** - defines models, columns, relationships, views, cubes, and metrics independent of the underlying warehouse.
- **Version-controlled business context** - enums, units, approved joins, and definitions live as Markdown/YAML in Git, reviewable like code.
- **Schema-aware retrieval and memory** - hybrid retrieval over a local LanceDB index plus structured error hints improve accuracy over time.
- **Agent and IDE integrations** - native skills for Claude Code, Cursor, Cline, Codex, and 50+ other agents via MCP, plus LangChain and Pydantic AI SDKs.
- **Dashboard generation** - agents can produce shareable dashboards and charts deployed to Vercel or Cloudflare Pages.

## Technology Stack
- **Languages:** Rust (core semantic engine `wren-core` on Apache DataFusion), Python (CLI/SDK `wrenai`, bindings `wren-core-py`), WebAssembly (`wren-core-wasm` for browser dashboards)
- **Dependencies:** Apache DataFusion, LanceDB, Hugging Face models (optional), Vercel/Cloudflare Pages for dashboard hosting
- **License:** Apache 2.0 (core engine, SDK, and skills are open source; some enterprise features such as row/column-level security and the hosted GenBI UI are commercial)

## GitHub Resources
- [Canner/WrenAI](https://github.com/Canner/WrenAI) - Open-source GenBI engine giving AI agents a governed semantic layer for text-to-SQL, dashboards, and charts across 20+ data sources.

## Related Skills
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
