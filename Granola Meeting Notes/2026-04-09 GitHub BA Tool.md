---
date: 2026-04-09
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-04-09

## Repository
- **Name:** WrenAI
- **GitHub URL:** https://github.com/Canner/WrenAI
- **Stars:** ⭐ 14,800+
- **License:** GNU AGPL v3.0
- **Last Updated:** 2025-03

## What It Does
WrenAI is an open-source Generative BI (GenBI) agent that lets anyone — including non-technical business analysts — query any database using plain English. Instead of writing SQL, you type a question like "What were the top 5 products by revenue last quarter?" and WrenAI translates it into accurate SQL, executes it, and renders the result as a chart or table in seconds. It supports 12+ data sources including PostgreSQL, BigQuery, Snowflake, MySQL, and DuckDB, and can be powered by any LLM including OpenAI, Claude, Gemini, or a locally-hosted Ollama model.

What makes WrenAI uniquely powerful compared to generic AI SQL tools is its semantic layer — a metadata definition language (MDL) where you encode your business definitions, metric formulas, and table relationships once. From that point forward, when you ask "What is our monthly churn rate?" the LLM knows exactly which tables, columns, and formulas define churn in your company's context, not a generic textbook definition. This eliminates the most common failure mode of text-to-SQL tools: generating syntactically valid SQL that answers the wrong question because the model guessed at business meaning.

WrenAI also generates spreadsheets and full BI reports from natural language prompts, and its entire pipeline runs with your data staying in your own infrastructure — nothing is uploaded to external LLM providers. For a BA working across multiple data systems, this is a self-hosted analytics co-pilot that speaks the same business language you use in requirements documents and stakeholder reports.

## Key Features
- Natural language to SQL: ask questions in plain English, get accurate query results
- Semantic layer (MDL) that stores your business metric definitions and table relationships
- Text-to-Chart: automatically visualizes query results as bar charts, line charts, and tables
- Spreadsheet and report generation from natural language prompts
- 12+ data source connectors (PostgreSQL, BigQuery, Snowflake, MySQL, DuckDB, etc.)
- LLM-agnostic: works with OpenAI, Claude, Gemini, or any local Ollama model
- Fully self-hostable — your data never leaves your infrastructure

## Installation
```bash
# Prerequisites: Docker and Docker Compose

# Clone the repository
git clone https://github.com/Canner/WrenAI.git
cd WrenAI

# Copy and configure environment variables
cp .env.example .env
# Edit .env to set your LLM provider API key and data source credentials

# Launch all services (UI, AI service, engine, postgres)
docker compose up -d

# WrenAI UI is now available at http://localhost:3000
# First-time setup wizard guides you through connecting your data source
# and defining your semantic layer (MDL)
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Self-Service Data Queries Without SQL Knowledge
Instead of raising a data request ticket to the BI team and waiting days for a report, open WrenAI and type your question in business language. Ask "Show me customer complaints by region this month" or "Which requirements have the most open change requests?" and get results instantly. Copy the output chart or table into your Obsidian requirements note or status report by exporting it as an image or CSV. This collapses the analysis-to-documentation cycle from days to minutes and lets a BA answer data questions in real time during stakeholder meetings.

### 2. Defining and Locking Down Business Metric Definitions
Use WrenAI's semantic layer (MDL) as the authoritative source for how your organisation defines KPIs. Work with the data team to encode definitions like "active user" (logged in within 30 days), "conversion rate" (trials that became paid accounts), or "defect rate" (bugs per story point). Once defined in MDL, every natural-language query about those metrics will use the agreed definition — not an improvised one. Link the MDL configuration file from your Obsidian data dictionary note as the canonical reference, so when stakeholders debate metric definitions during a workshop, you can point to a living, versioned source of truth.

### 3. Rapid Acceptance Criteria Validation with Real Data
After writing acceptance criteria for a user story, use WrenAI to query the connected test or staging database and verify that the underlying data actually supports the expected behaviour. For example, if an AC states "All orders placed before 5pm ship same day", query the orders table in natural language to check what percentage of current orders would pass that rule. Paste the result directly into the AC section of your Obsidian story card with a timestamp, so testers and developers know the AC was validated against real data before sprint start, not just written in the abstract.

### 4. Stakeholder Reporting Without a BI Developer
When a stakeholder requests a one-off metric for a steering committee presentation, use WrenAI to generate the chart or table on the fly rather than waiting for a BI developer to build a dashboard. Ask "Give me a month-over-month trend of new registrations for the last 6 months" and export the generated chart directly into your Obsidian weekly reporting note. Attach the auto-generated SQL alongside the chart so developers can later productionise the exact query if it becomes a recurring report — the BA becomes a bridge between the business question and the technical implementation.

### 5. Discovery Analysis During Requirements Elicitation
During the discovery phase of a new project, use WrenAI to explore an existing system's data before writing requirements. Ask exploratory questions like "What are the most common values in the status field of the orders table?" or "How many records have null values in the customer_id column?" to understand data quality issues and edge cases before they surface during UAT. Document your findings in an Obsidian data discovery note linked to the project epic — these pre-flight observations inform your requirements with real constraints and prevent surprises late in the delivery cycle.

## Why This Tool Today
None of the previously discovered tools give a BA direct, self-service access to live data. Metabase provides dashboards but still requires a data team to build them; ydata-profiling works on static files, not live databases. WrenAI fills the gap by letting a BA query any live database in plain English with zero SQL knowledge, using a semantic layer that enforces the business's own metric definitions — turning data access from a bottleneck into a BA superpower.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
