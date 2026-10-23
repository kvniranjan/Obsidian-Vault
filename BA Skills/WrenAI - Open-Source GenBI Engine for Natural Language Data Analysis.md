---
date: 2026-10-23
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, text-to-sql, genbi, ai-assisted-ba, decision-management]
source: GitHub
---

# WrenAI - Open-Source GenBI Engine for Natural Language Data Analysis

## What is it?
WrenAI (Canner/WrenAI) is an open-source Generative BI (GenBI) engine that lets AI agents answer business questions in natural language by generating governed SQL against a defined semantic layer. Instead of writing raw SQL or exploratory queries by hand, users (or AI agents such as Claude Code, Cursor, or any MCP client) ask a question and WrenAI plans, validates, and executes a query against connected data sources, then can turn the result into a dashboard or chart. Business definitions, enums, and approved joins are stored as version-controlled YAML and Markdown, so the semantic layer (called MDL) is reviewable like code.

## Why it matters for Business Analysts
BAs are frequently the bridge between stakeholder questions and the data needed to answer them, but often lack direct SQL skills or must wait on data/BI teams for every ad-hoc request. WrenAI lets a BA describe a business question in plain language and get back a governed, explainable query and visualization, without bypassing data governance rules the team has already defined. Because the semantic layer (business terms, metrics, approved joins) is stored as Git-versioned files, BAs can directly review, propose, and track changes to how business concepts map to underlying data — much like maintaining a requirements or glossary document. It also supports rapid validation of hypotheses during requirements elicitation or process analysis by making ad-hoc data analysis self-service.

## How to use it in BA Workflows
1. **Self-service business question answering** - Ask natural-language questions ("What were our top 5 customers by revenue last quarter?") and get back governed SQL plus a result set, without needing to write SQL or file a ticket with a data team.
2. **Data-driven requirements validation** - When gathering requirements, use WrenAI to quickly pull real data (volumes, distributions, exceptions) that validates or challenges assumptions stakeholders are making, grounding requirements in evidence.
3. **Maintaining a business glossary as code** - Treat the MDL (semantic layer) files as a living business glossary: BAs can propose new business term definitions, metrics, or approved joins via pull request, keeping terminology consistent across the organization.
4. **Rapid dashboard prototyping for stakeholders** - Use agent-built dashboards (deployable to Vercel/Cloudflare Pages) to quickly produce a shareable view of a KPI or process metric for stakeholder review sessions, rather than waiting on a full BI build cycle.
5. **AI-agent-assisted analysis in existing BA tooling** - Because WrenAI integrates with MCP clients, LangChain, Claude Code, and Cursor, BAs can wire it into their existing AI-assisted workflows (e.g., alongside requirements or process-modeling assistants) so that data questions arising mid-analysis can be answered inline.

## Key Features
- Text-to-SQL planning against a semantic layer (MDL) with dry-plan validation and row limits, reducing risk of ungoverned or runaway queries
- Business definitions, enums, and approved joins stored as version-controlled YAML/Markdown for transparent, auditable semantics
- Native integration with AI agent ecosystems: Claude Code, Cursor, MCP clients, and LangChain
- Broad connector support (20+ data sources including BigQuery, Snowflake, PostgreSQL, ClickHouse, Redshift, Databricks, DuckDB) via an Apache DataFusion engine
- Agent-built dashboards deployable as standalone browser-side apps
- CLI (`wren query`, `wren ask`) for scripting and automation of data questions
- Open-core model: core engine, SDK, and skills are Apache 2.0; enterprise features (row/column-level security, GenBI UI, Git Sync) are commercial

## Technology Stack
- **Languages:** Rust (semantic/query engine), Python (SDK/CLI)
- **Dependencies:** Apache DataFusion (query execution engine), MDL semantic layer format (YAML/Markdown)
- **License:** Apache 2.0 (core engine, SDK, skills); AGPL-3.0 and CC-BY-4.0 apply to select other components

## GitHub Resources
- [Canner/WrenAI](https://github.com/Canner/WrenAI) - Open-source GenBI engine that turns natural-language questions into governed SQL, dashboards, and charts

## Related Skills
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[WhoDB - AI-Powered Database Exploration with Text-to-SQL and ER Diagrams]]
