---
date: 2026-09-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, data-transformation, analytics-engineering, sql, business-intelligence]
source: GitHub
---

# dbt Core - SQL-Based Data Transformation and Analytics Engineering Framework

## What is it?
dbt (data build tool) Core is an open-source command-line framework that lets analysts and engineers transform raw data already loaded into a warehouse using plain SQL `select` statements. It compiles those statements into tables and views, manages dependencies between models, and applies software-engineering practices — version control, testing, documentation, and CI/CD — to the analytics layer.

## Why it matters for Business Analysts
BAs are increasingly asked to define, validate, and document the business logic behind KPIs and reporting metrics, not just consume dashboards built by data engineers. dbt gives BAs a low-barrier, SQL-only way to own that logic directly: defining metrics, data quality tests, and documentation as version-controlled code that both technical and business stakeholders can review. Its auto-generated documentation and lineage graphs make it easy to trace exactly how a business metric was derived, which is invaluable during requirements validation and stakeholder sign-off. Because models are just SQL, BAs can collaborate with data teams using a shared, auditable source of truth instead of ad hoc spreadsheet logic.

## How to use it in BA Workflows
1. **Metric Definition** - Translate business requirements (e.g., "monthly active customers", "net revenue retention") into dbt models so the calculation logic is centralized, tested, and reusable across reports.
2. **Data Quality & Assumption Testing** - Use dbt's built-in and custom tests (uniqueness, not-null, referential integrity, accepted values) to codify and continuously validate business rules and assumptions gathered during elicitation.
3. **Requirements Traceability for Reporting** - Use the auto-generated lineage graph (`dbt docs generate`) to show stakeholders exactly which source systems and transformations feed a given report or KPI, supporting impact analysis for change requests.
4. **Stakeholder Documentation** - Write model and column descriptions in YAML alongside the SQL so definitions of business terms live next to the logic that implements them, reducing ambiguity between BAs, analysts, and engineers.
5. **Change Impact Analysis** - Before approving a change to a data source or metric definition, use `dbt build --select +model+` to see every downstream report and model affected, supporting more rigorous change control.

## Key Features
- SQL-first modeling with Jinja templating for reusable, parameterized transformation logic
- Built-in testing framework for enforcing business and data-quality rules
- Automatic dependency resolution and DAG-based lineage visualization
- Auto-generated, searchable documentation site for data definitions
- Version control and CI/CD-friendly workflow (git-based development)
- Broad adapter ecosystem supporting Snowflake, BigQuery, Databricks, Redshift, Postgres, and more

## Technology Stack
- **Languages:** Python, SQL, Jinja
- **Dependencies:** A supported data warehouse/database (Snowflake, BigQuery, Databricks, Redshift, Postgres, etc.) via dbt adapters
- **License:** Apache License 2.0

## GitHub Resources
- [dbt-labs/dbt-core](https://github.com/dbt-labs/dbt-core) - Open-source engine for transforming data in the warehouse using SQL and software-engineering practices

## Related Skills
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[OpenLineage - Open Standard for Data Pipeline Lineage Tracking]]
- [[DataHub - Open-Source AI Data Catalog and Governance Platform]]
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
