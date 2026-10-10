---
date: 2026-10-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, ai-assisted, text-to-sql, business-intelligence, natural-language, llm]
source: GitHub
---

# WrenAI - Open-Source GenBI Agent for Natural Language Data Analysis

## What is it?
WrenAI is an open-source "GenBI" (Generative Business Intelligence) agent that lets anyone query a database in plain natural language and get back accurate SQL (Text-to-SQL), charts (Text-to-Charts), and AI-generated insights. It is built from three components — a web UI, an AI service that retrieves schema context from a vector database to ground the LLM, and a semantic engine ("Wren Engine") that maps business terminology to the underlying data model via a Modeling Definition Language (MDL). With roughly 15,000 GitHub stars, it supports a wide range of warehouses including BigQuery, Snowflake, Redshift, PostgreSQL, MySQL, ClickHouse, Oracle, and Trino.

## Why it matters for Business Analysts
Business Analysts are frequently the translation layer between raw data and business meaning, and WrenAI's semantic layer (MDL) is designed to encode exactly that translation — business terms, relationships, and calculation logic — so that questions phrased in business language resolve to the correct SQL rather than relying on an analyst to hand-write every query. This lets BAs self-serve data validation, trend analysis, and KPI exploration during requirements gathering without waiting on data engineering support. Because the semantic model is explicit and reusable, it also doubles as living documentation of business definitions (e.g., what counts as "active customer" or "net revenue"), reducing ambiguity across stakeholder conversations. The ability to produce both SQL and charts from one natural-language prompt makes it well suited to live stakeholder workshops and rapid as-is analysis.

## How to use it in BA Workflows
1. **Requirements Validation via Live Data** - Ask natural-language questions against the production warehouse ("How many orders were cancelled in each region last quarter?") to sanity-check assumptions before finalizing requirements or acceptance criteria.
2. **Semantic Model as Business Glossary** - Build out the MDL semantic layer collaboratively with stakeholders so that business terms (e.g., "churned customer", "gross margin") have one authoritative, data-grounded definition that BAs can reference in specs.
3. **Stakeholder Workshops and Demos** - Use the Text-to-SQL and Text-to-Charts capability live in workshops to answer ad-hoc stakeholder questions ("Show me a trend of support tickets by category this year") without pre-building dashboards.
4. **Gap and Root-Cause Analysis** - Drill into anomalies surfaced during process analysis (e.g., unexpected spikes in a metric) by iteratively asking follow-up natural-language questions against the same semantic model.
5. **KPI and Metric Discovery** - Explore candidate KPIs and their historical baselines across multiple warehouses before writing them into a business case or BRD, ensuring the metric defined in the spec matches what the semantic layer can actually compute.

## Key Features
- **Text-to-SQL and Text-to-Charts** - Converts natural-language business questions directly into executable SQL and corresponding visualizations
- **Semantic layer (MDL)** - A Modeling Definition Language that encodes business terminology, relationships, and calculation logic so the LLM reasons over business meaning, not raw schema
- **Multi-warehouse support** - Works with BigQuery, Snowflake, Redshift, PostgreSQL, MySQL, ClickHouse, Oracle, Trino, DuckDB, and SQL Server
- **Retrieval-grounded reasoning** - The AI service retrieves relevant schema/semantic context from a vector database before generating SQL, reducing hallucinated queries
- **Modular architecture** - Separate UI, AI service, and semantic engine components allow embedding into existing BI stacks or custom tooling
- **Self-hostable** - Fully deployable via Docker for teams with data residency or governance requirements

## Technology Stack
- **Languages:** Python (AI service), TypeScript/Node.js (Wren UI), Java (Wren Engine)
- **Dependencies:** Vector database for schema retrieval, Docker Compose for deployment, pluggable LLM backends (OpenAI and others)
- **License:** AGPL-3.0 (core project); separate commercial "Wren AI Cloud" offering

## GitHub Resources
- [Canner/WrenAI](https://github.com/Canner/WrenAI) - Open-source GenBI agent providing Text-to-SQL, Text-to-Charts, and a business semantic layer; ~15k stars

## Related Skills
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[DeepAnalyze - Agentic LLM for Autonomous Data Science and Reporting]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
