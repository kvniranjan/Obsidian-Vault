---
date: 2026-07-06
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-lineage, metadata, data-governance, data-catalog, pipeline, open-standard, compliance]
source: GitHub
---

# OpenLineage - Open Standard for Data Pipeline Lineage Tracking

## What is it?
OpenLineage is an open standard and framework for collecting lineage metadata from data pipelines as they run. It defines a vendor-neutral specification (built on OpenAPI) that captures which datasets a job reads and writes, how data transforms between them, and the provenance of every pipeline run. It is a Linux Foundation AI & Data Foundation graduate project with 2,500+ stars and integrations for Spark, Airflow, dbt, Flink, Dagster, and more.

## Why it matters for Business Analysts
BAs routinely need to answer questions like "if this source table changes, what reports break?" or "where did this data quality issue originate?" — OpenLineage makes those answers traceable rather than guesswork. It provides end-to-end visibility into how raw data flows through transformation layers all the way to dashboards and decision-support systems, directly supporting impact analysis and change management work. For regulated industries, the captured lineage events serve as auditable evidence that data handling meets compliance requirements (GDPR, BCBS 239, etc.). Because it is an open standard rather than a proprietary tool, BAs can reference lineage metadata stored in any compatible backend (Marquez, DataHub, OpenMetadata) without vendor lock-in.

## How to use it in BA Workflows
1. **Impact Analysis for Change Requests** - When a source system or schema change is proposed, query the lineage graph to enumerate all downstream jobs, datasets, and reports that will be affected. Present the impact map to stakeholders before sign-off to avoid surprise regressions.
2. **Data Quality Root Cause Investigation** - When a KPI or report shows unexpected values, traverse lineage upstream from the output dataset to identify which pipeline stage introduced the anomaly, narrowing scope for the development team.
3. **Regulatory Data Flow Documentation** - Export lineage metadata as documentation showing auditors exactly how personal or sensitive data moves through systems, satisfying data-flow mapping requirements under privacy regulations.
4. **Requirements Validation for Data Products** - After new pipeline requirements are delivered, verify that the implemented lineage matches the agreed data flow diagrams — confirming that all required source fields are read and all required output fields are produced.
5. **Stakeholder Data Flow Diagrams** - Use lineage data as the authoritative source for automatically generating business-readable data flow diagrams, replacing manually maintained (and often stale) architecture documents.

## Key Features
- **Open specification** — OpenAPI-defined event model covering run, job, and dataset entities; extensible via custom facets for domain-specific metadata
- **Real-time collection** — emits events at job start, complete, and fail so lineage is captured as pipelines execute, not reconstructed after the fact
- **Column-level lineage** — traces individual field transformations across datasets, enabling fine-grained impact analysis
- **Broad integrations** — official integrations for Apache Spark, Apache Airflow, dbt, Apache Flink, Dagster, Trino, and more
- **Multi-language clients** — Python, Java, and Go client libraries for instrumenting custom pipelines
- **Backend agnostic** — emits events to any compatible backend (Marquez, DataHub, OpenMetadata) via a standard HTTP API
- **Vendor neutral** — LF AI & Data Foundation graduate project; no single vendor controls the specification

## Technology Stack
- **Languages:** Java (core integrations), Python (Airflow, dbt integrations; client library), Go (client library)
- **Dependencies:** OpenAPI 3 specification; integrations depend on respective platform SDKs (PySpark, Airflow providers, dbt adapters)
- **License:** Apache License 2.0

## GitHub Resources
- [OpenLineage/OpenLineage](https://github.com/OpenLineage/OpenLineage) - Open standard and reference integrations for data pipeline lineage metadata collection

## Related Skills
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[Amundsen - Metadata-Driven Data Discovery Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[DeepAnalyze - Agentic LLM for Autonomous Data Science and Reporting]]
