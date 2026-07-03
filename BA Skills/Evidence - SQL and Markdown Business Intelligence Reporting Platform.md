---
date: 2026-07-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, business-intelligence, reporting, sql, markdown, data-visualization, stakeholder-reporting]
source: GitHub
---

# Evidence - SQL and Markdown Business Intelligence Reporting Platform

## What is it?
Evidence is an open-source, code-driven business intelligence framework that lets you build polished, interactive data reports and dashboards using SQL queries and Markdown — no drag-and-drop required. Reports are written like documents, with SQL blocks embedded directly in Markdown files, and charts and tables rendered automatically from the query results. The output is a fast, shareable static web app that connects live to your data warehouse.

## Why it matters for Business Analysts
BAs constantly need to communicate data-driven insights to stakeholders, but traditional BI tools either require expensive licenses or produce dashboards that are hard to document and version-control. Evidence bridges the gap by treating reports as code: SQL queries capture the logic, Markdown explains the narrative, and Git manages the history — so any analyst who knows SQL can build and maintain professional-quality reports. Stakeholder deliverables become reproducible artifacts rather than one-off exports, enabling auditable, collaborative analysis workflows. The tool supports all major data sources (BigQuery, Snowflake, Redshift, DuckDB, PostgreSQL, and more), making it easy to integrate into existing data stacks without a heavy setup burden.

## How to use it in BA Workflows
1. **Stakeholder Reporting** - Replace static PowerPoint slide decks or PDF exports with living Evidence reports that auto-refresh from the source database, ensuring stakeholders always see current figures without manual updates.
2. **Requirements Validation with Data** - Embed SQL queries that directly validate acceptance criteria — for example, confirming that a process change produced the expected outcome in production data — and share the report as documented proof.
3. **Ad-hoc Data Analysis** - Write exploratory SQL analyses alongside narrative Markdown commentary to capture the reasoning behind findings, then publish the report to a URL for instant stakeholder review.
4. **KPI and Metrics Dashboards** - Build self-service dashboards for business owners that surface key metrics (SLA adherence, defect rates, process throughput) without requiring a dedicated BI engineer for every new request.
5. **Data-Driven BRD Annexes** - Attach Evidence report links or export snapshots as appendices to Business Requirement Documents, providing live, verifiable data context to support business case arguments.

## Key Features
- **SQL-first queries** — embed parameterised SQL blocks directly in Markdown pages; no proprietary query language
- **Built-in chart components** — line, bar, scatter, area, funnel, heatmap, and more, all rendered from query results with a single component tag
- **Multiple data source connectors** — BigQuery, Snowflake, Redshift, DuckDB, PostgreSQL, MySQL, SQLite, CSV, and community connectors
- **Static site output** — reports compile to a fast static web app, hostable on any static host (Vercel, Netlify, GitHub Pages)
- **Git-native workflow** — reports live in a repo, enabling pull-request reviews, branching, and CI/CD-based publishing
- **Templated pages** — a single Markdown template can generate one page per product, region, or entity using loop variables
- **Live data refresh** — optional server mode keeps dashboards current by re-running queries on a schedule

## Technology Stack
- **Languages:** JavaScript / TypeScript (SvelteKit), SQL, Markdown
- **Dependencies:** Node.js; optional DuckDB for local file-based queries
- **License:** MIT

## GitHub Resources
- [evidence-dev/evidence](https://github.com/evidence-dev/evidence) - Build fast, interactive data visualizations in SQL and Markdown

## Related Skills
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[Amundsen - Metadata-Driven Data Discovery Platform]]
