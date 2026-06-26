---
date: 2026-06-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, data-catalog, data-discovery, metadata, data-governance, data-lineage]
source: GitHub
---

# Amundsen - Metadata-Driven Data Discovery Platform

## What is it?
Amundsen is an open-source, metadata-driven data discovery and exploration application incubated by the Linux Foundation AI & Data Foundation. Originally built at Lyft, it indexes metadata from databases, dashboards, and data pipelines to create a searchable catalog of all data assets in an organization. Users can find, understand, and trust data through rich context including ownership, usage frequency, quality scores, and lineage.

## Why it matters for Business Analysts
BAs frequently waste significant time hunting for the right data to support requirements, impact assessments, or feasibility studies — Amundsen solves this by making every data asset in the organization searchable in seconds. It surfaces who owns a dataset, how often it's used, and where the data comes from, giving BAs the confidence to cite data sources accurately in specifications and reports. The platform's popularity scores (based on query frequency) help BAs identify authoritative, well-trusted datasets over obscure or stale ones. For BAs bridging the gap between business stakeholders and data teams, Amundsen serves as a shared vocabulary — a place where business-friendly descriptions and technical metadata coexist.

## How to use it in BA Workflows
1. **Requirements data sourcing** - Before writing data-related requirements, search Amundsen to locate candidate tables or dashboards, review their descriptions and ownership, and confirm the right data exists to support the proposed feature.
2. **Impact analysis** - When a business change may affect reporting or data flows, use Amundsen's lineage views to trace upstream sources and downstream consumers, identifying all affected systems and teams before documenting scope.
3. **Stakeholder data interviews** - Share Amundsen search results with subject-matter experts during workshops to anchor conversations on specific, named datasets rather than vague references, reducing miscommunication.
4. **Data quality and trust assessment** - Review table-level metadata (last updated, row counts, quality badges) to flag unreliable data sources early in the analysis phase, preventing downstream specification errors.
5. **Glossary and business term alignment** - Use Amundsen's description fields and tagging to cross-reference technical column names with business terminology, building a living data dictionary that both analysts and developers can reference.

## Key Features
- Full-text search across tables, dashboards, users, and tags with ranked results by popularity
- Table detail pages showing schema, sample data, owners, frequent users, and descriptions
- Data lineage graph tracing data flow across pipelines and transformations
- Integration with major data warehouses (BigQuery, Snowflake, Redshift, Hive, Presto)
- Slack and email notifications for dataset changes affecting subscribed users
- Crowdsourced metadata: any user can add descriptions, tags, and owners to improve discoverability
- Native support for Amundsen DataBuilder ETL pipelines to ingest metadata from 30+ sources

## Technology Stack
- **Languages:** Python (backend/metadata ingestion), TypeScript/React (frontend)
- **Dependencies:** Neo4j (graph database for lineage), Elasticsearch (search index), Apache Atlas (optional metadata store)
- **License:** Apache 2.0

## GitHub Resources
- [amundsen-io/amundsen](https://github.com/amundsen-io/amundsen) - Metadata-driven data discovery application for improving data analyst productivity

## Related Skills
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
