---
date: 2026-07-05
type: skill
category: Business Analysis
tags: [business-analyst, skill, data-analysis, ai, llm, agentic-ai, data-science, reporting, automation]
source: GitHub
---

# DeepAnalyze - Agentic LLM for Autonomous Data Science and Reporting

## What is it?
DeepAnalyze is an open-source agentic LLM platform built by Renmin University's data lab that autonomously completes end-to-end data science tasks without manual intervention. It supports structured data (CSV, Excel, databases), semi-structured data (JSON, XML), and unstructured data (TXT, Markdown), covering the full pipeline from data preparation and analysis through modeling, visualization, and professional report generation. The project ships an open-source model (DeepAnalyze-8B) alongside the framework, making it fully self-hostable.

## Why it matters for Business Analysts
Business Analysts routinely spend hours cleaning datasets, writing ad-hoc queries, and assembling stakeholder reports — DeepAnalyze automates that entire loop in a conversational interface. It can interrogate multiple data sources simultaneously, surface patterns and anomalies a human might miss across large volumes of rows, and produce analyst-grade research reports ready for executive review. Because the model and inference code are fully open-source under the MIT license, teams can fine-tune it on proprietary domain data, ensuring outputs align with organisational terminology and KPIs rather than generic statistics.

## How to use it in BA Workflows
1. **Rapid data profiling** - Point DeepAnalyze at a raw CSV or database export and ask it to profile the dataset: column distributions, missing values, outliers, and data-quality issues are surfaced as a structured report before any formal analysis begins.
2. **Stakeholder report generation** - Provide business questions in plain language (e.g., "Why did conversion rates drop in Q2?") and DeepAnalyze produces a narrative report with embedded charts, statistical evidence, and interpretive commentary — ready to share with non-technical stakeholders.
3. **Multi-source data reconciliation** - Feed it structured exports from multiple systems (CRM, ERP, analytics) and ask cross-cutting questions; it joins, reconciles, and analyses across sources without requiring a BA to write SQL or Python manually.
4. **Requirements evidence gathering** - Use DeepAnalyze to mine historical transaction logs or usage data to produce quantitative evidence that supports or challenges proposed system requirements, giving BA artefacts an empirical grounding.
5. **Deep research on business domains** - Ask DeepAnalyze to research an industry topic by combining internal data with provided documents, generating a cited, multi-section report that accelerates the discovery phase of a new project.

## Key Features
- **Full pipeline automation** - Handles data prep, analysis, modelling, visualization, and report generation in a single agentic loop
- **Multi-format data support** - Reads structured (CSV, Excel, SQL databases), semi-structured (JSON, XML, YAML), and unstructured (Markdown, TXT) sources
- **DeepAnalyze-8B open model** - Fully open-source fine-tuned model deployable on local or cloud infrastructure
- **Jupyter integration** - Generates and executes Jupyter notebook cells, making outputs reproducible and auditable
- **Analyst-grade reports** - Produces professional, narrative-style HTML/Markdown reports with embedded visualizations
- **Deep research mode** - Can combine multiple data sources and produce multi-section, cited research documents

## Technology Stack
- **Languages:** Python
- **Dependencies:** Qwen-series LLMs (default), Jupyter kernel, pandas, matplotlib/plotly for visualization
- **License:** MIT

## GitHub Resources
- [ruc-datalab/DeepAnalyze](https://github.com/ruc-datalab/DeepAnalyze) - Agentic LLM for autonomous data science with 4,300+ stars

## Related Skills
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[OpenMetadata - Unified Data Discovery and Governance Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[Flowise - Visual AI Agent and Workflow Builder]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
