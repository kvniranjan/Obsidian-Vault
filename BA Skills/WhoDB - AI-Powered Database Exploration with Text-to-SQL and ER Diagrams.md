---
date: 2026-07-17
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, text-to-sql, ai-assistant, database, er-diagram, data-catalog, data-governance]
source: GitHub
---

# WhoDB - AI-Powered Database Exploration with Text-to-SQL and ER Diagrams

## What is it?
WhoDB is an open-source, self-hosted database management and exploration tool that combines AI-assisted natural language querying (text-to-SQL), interactive ER diagram generation, a visual query builder, and data catalog features in a single lightweight interface. It supports multiple database engines including MySQL, PostgreSQL, SQLite, Oracle, and SQL Server, and exposes an MCP server for AI agent integration. Created in June 2024, it has rapidly attracted nearly 5,000 GitHub stars.

## Why it matters for Business Analysts
BAs frequently need to explore unfamiliar databases to understand data models, validate requirements, and extract insights — but are often limited by SQL proficiency or access to dedicated BI tools. WhoDB removes that barrier by letting analysts query data in plain English, with AI translating the intent into correct SQL. The ER diagram generation gives BAs an immediate visual map of table relationships, which is invaluable for data dictionary creation, gap analysis, and communicating data structures to stakeholders. Its self-hosted, zero-dependency design means teams can deploy it quickly without procurement hurdles, and the MCP server integration allows AI agents and copilots to query operational data as part of automated BA workflows.

## How to use it in BA Workflows
1. **Data Discovery During Requirements Gathering** - Deploy WhoDB against a target database and use natural language queries ("Show me all customer orders placed in the last 90 days with their statuses") to rapidly explore data without needing to know the schema upfront, reducing time spent in discovery interviews just to understand existing data structures.
2. **Automated ER Diagram Generation for Data Dictionary Creation** - Use the built-in ER diagram feature to generate visual entity-relationship maps of any connected database, then export and embed them in requirements documents, BRDs, or data dictionaries to give developers and stakeholders shared context.
3. **Data Validation and Acceptance Criteria Testing** - Run ad-hoc natural language queries to validate that data transformations or migrations meet acceptance criteria (e.g., "Find any customer records missing a valid email address"), surfacing data quality issues early without waiting for formal QA cycles.
4. **Stakeholder Data Storytelling** - Use the visual query builder and built-in charting to rapidly compose data snapshots for stakeholder presentations, replacing the need to hand off data requests to engineering or BI teams for simple exploratory questions.
5. **AI-Agent Integration via MCP** - Connect WhoDB's MCP server to an AI copilot (Claude, Cursor, etc.) so that automated BA agents can query live operational data during requirements analysis, process validation, or impact assessment tasks — bridging natural language analysis and structured data.

## Key Features
- **Text-to-SQL**: Natural language interface translates plain English questions into SQL queries across all connected databases
- **ER Diagram Generator**: Auto-generates visual entity-relationship diagrams for any schema, exportable for documentation
- **Visual Query Builder**: Point-and-click query construction for non-SQL users, with filter, sort, and join support
- **Multi-Database Support**: MySQL, PostgreSQL, SQLite, Oracle, SQL Server, and more from a single interface
- **MCP Server**: Exposes database access to AI agents and copilots via the Model Context Protocol
- **Data Catalog**: Browse tables, columns, and metadata across connected databases with search
- **Data Governance Visibility**: Surface data lineage, relationships, and ownership context
- **Self-Hosted and Lightweight**: Runs as a single Go binary or Docker container with no external dependencies
- **AI Agent Integration**: Built-in AI agent for autonomous data exploration and analysis tasks

## Technology Stack
- **Languages:** Go (backend), TypeScript/React (frontend)
- **Dependencies:** Docker-deployable; supports major SQL databases natively
- **License:** Apache 2.0

## GitHub Resources
- [clidey/whodb](https://github.com/clidey/whodb) - AI-powered database exploration with text-to-SQL, ER diagrams, and MCP integration

## Related Skills
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[DeepAnalyze - Agentic LLM for Autonomous Data Science and Reporting]]
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[Amundsen - Metadata-Driven Data Discovery Platform]]
- [[OpenLineage - Open Standard for Data Pipeline Lineage Tracking]]
