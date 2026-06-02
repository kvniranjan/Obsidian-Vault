---
date: 2026-06-02
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-catalog, data-governance, data-lineage, metadata, data-discovery, data-observability]
source: GitHub
---

# DataHub - Open-Source AI Data Catalog and Governance Platform

## What is it?
DataHub is an open-source metadata platform originally created at LinkedIn that serves as a centralized catalog for discovering, understanding, and governing an organization's data assets. It ingests metadata from 80+ data sources — databases, data warehouses, BI tools, pipelines, and ML models — and presents them through a unified search and lineage interface. The project has over 11,800 GitHub stars and is used in production at companies like Airbnb, Grab, and Coursera.

## Why it matters for Business Analysts
BAs frequently struggle to locate authoritative data sources, understand what data means, and assess the downstream impact of data changes — DataHub directly solves all three problems in one tool. Its business glossary feature lets BAs attach organization-wide definitions to datasets and columns, bridging the gap between technical schemas and business terminology. Column-level lineage allows BAs to trace exactly where data originates and which reports, dashboards, or pipelines depend on a given field, making impact analysis fast and accurate. Governance dashboards let BAs work with data stewards to assign ownership, classify sensitivity, and enforce compliance — critical for regulated-industry BA work.

## How to use it in BA Workflows
1. **Data asset discovery** - Use the universal search to find tables, dashboards, or pipeline outputs relevant to a requirements investigation; filter by domain, owner, or tag rather than asking engineers which table to use.
2. **Impact analysis for requirements changes** - Before documenting a proposed change to a source system field, trace its downstream lineage in DataHub to identify every report, dashboard, or downstream dataset that would be affected — and include those in the change impact section of your BRD.
3. **Business glossary authoring** - Collaboratively define and publish canonical business terms (e.g., "Active Customer", "Gross Revenue") linked to the physical columns that implement them, ensuring the requirements specification and the data model share consistent language.
4. **Data documentation and context gathering** - Add dataset descriptions, column-level annotations, and "how to use" notes directly in DataHub during discovery phases so future BA and analyst work starts with pre-documented context instead of tribal knowledge.
5. **Data governance and compliance mapping** - Assign data ownership, sensitivity classifications, and compliance tags (PII, GDPR, HIPAA) to datasets discovered during requirements elicitation, supporting privacy impact assessments and regulatory requirement tracing.

## Key Features
- **Universal search** — Full-text and faceted search across all ingested data assets, with relevance tuned by usage statistics
- **Column-level lineage** — Visual graph tracing data flow from source tables through transformations to BI dashboards
- **Business glossary** — Managed vocabulary of business terms linked to physical data assets and columns
- **Data profiling** — Automated schema statistics, null rates, and value distributions surfaced alongside dataset metadata
- **Governance dashboard** — Policy management, ownership assignment, and compliance tagging at scale
- **80+ production connectors** — Native ingestion from Snowflake, BigQuery, dbt, Airflow, Looker, Tableau, Kafka, and more
- **GraphQL & REST APIs** — Programmatic access for embedding DataHub context in other BA tooling or documentation workflows

## Technology Stack
- **Languages:** Python (ingestion framework), Java (backend GMS service), TypeScript/React (frontend)
- **Dependencies:** Elasticsearch, Kafka, MySQL/PostgreSQL, Neo4j (optional lineage graph)
- **License:** Apache License 2.0

## GitHub Resources
- [datahub-project/datahub](https://github.com/datahub-project/datahub) - The Context Platform for your Data and AI Stack; unified metadata, lineage, and governance for 80+ data sources

## Related Skills
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
