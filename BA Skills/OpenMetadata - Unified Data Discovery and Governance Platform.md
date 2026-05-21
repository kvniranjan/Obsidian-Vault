---
date: 2026-05-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-governance, data-catalog, data-lineage, metadata, data-analysis, data-discovery]
source: GitHub
---

# OpenMetadata - Unified Data Discovery and Governance Platform

## What is it?
OpenMetadata is an open-source, unified metadata platform built for data discovery, data observability, and data governance. It provides a central metadata repository with in-depth column-level data lineage, a business glossary, and 120+ built-in connectors to popular data sources, warehouses, and pipelines. It combines AI-powered semantic search with rich collaboration features so data teams can document, govern, and share understanding of their data assets.

## Why it matters for Business Analysts
Business Analysts are often the bridge between data assets and business requirements — they need to quickly locate relevant data, understand its meaning, and confirm its quality before using it in analysis or defining requirements. OpenMetadata gives BAs a searchable data catalog so they can self-serve answers about what data exists, who owns it, and how it has been transformed. The built-in data lineage viewer lets BAs trace how a metric or report value is derived end-to-end, which is critical for impact analysis when requirements change. The business glossary feature lets BAs define and own canonical business terms that data engineers, analysts, and stakeholders all reference, eliminating the costly ambiguity that comes from inconsistent terminology across teams.

## How to use it in BA Workflows
1. **Data Asset Discovery** - Use the AI-powered semantic search to find tables, dashboards, pipelines, and topics by business concept (e.g., "customer churn") rather than exact technical names, saving hours spent hunting through data warehouses.
2. **Impact Analysis** - Before drafting a change request, use the column-level lineage graph to trace all downstream reports, dashboards, and pipelines that depend on a data source, so the full blast radius of a change is understood upfront.
3. **Business Glossary Management** - Create and maintain a glossary of authoritative business terms (e.g., "Active Customer", "Revenue") directly in OpenMetadata, linking them to the physical table columns they map to so requirements and data definitions stay in sync.
4. **Data Quality Validation** - Review data profiling statistics and quality test results attached to tables before including data in analysis, reducing the risk of presenting stakeholders with metrics derived from incomplete or erroneous data.
5. **Stakeholder Collaboration on Data Documentation** - Use inline comments, task assignments, and rich-text descriptions to collaboratively document data assets alongside engineers and stewards, building a shared understanding that reduces back-and-forth in requirements sessions.

## Key Features
- **120+ Connectors** - Out-of-the-box ingestion from databases, data warehouses, BI tools, ML platforms, and messaging systems
- **Column-Level Lineage** - Visual end-to-end lineage with no-code manual editing for documenting undocumented pipelines
- **Business Glossary** - Define, approve, and link canonical business terms to physical data assets
- **Data Profiling & Quality** - Automated profiling statistics and configurable quality tests surfaced per table
- **AI Semantic Search** - Meaning-based search returns conceptually related assets even without exact keyword matches
- **Data Insights & KPIs** - Platform analytics dashboards to track documentation coverage, ownership, and tiering goals
- **Roles & Policies** - Granular access control with teams, roles, and data-tier classifications

## Technology Stack
- **Languages:** Java (backend), TypeScript/React (frontend), Python (ingestion framework)
- **Dependencies:** Elasticsearch/OpenSearch, MySQL/PostgreSQL, Airflow (optional pipeline orchestration)
- **License:** Apache 2.0

## GitHub Resources
- [open-metadata/OpenMetadata](https://github.com/open-metadata/OpenMetadata) - Unified metadata platform for data discovery, observability, and governance with 120+ connectors and column-level lineage

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[n8n - Fair-Code Workflow Automation Platform]]
