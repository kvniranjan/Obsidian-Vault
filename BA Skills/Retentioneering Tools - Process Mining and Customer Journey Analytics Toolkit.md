---
date: 2026-07-15
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, customer-journey, behavioral-analytics, data-analysis, ai-assisted, mcp-server]
source: GitHub
---

# Retentioneering Tools - Process Mining and Customer Journey Analytics Toolkit

## What is it?
Retentioneering Tools is an open-source Python toolkit for reproducible, auditable clickstream and event log analytics. It enables analysts to build, validate, and cross-check customer journeys, graph-based user flows, behavioral segmentation, A/B tests, and process mining models from event data. It recently expanded to include an MCP server and agent skills, making it directly usable in AI-assisted analysis pipelines.

## Why it matters for Business Analysts
BAs increasingly need to validate that real user behavior matches designed business processes — Retentioneering bridges that gap by mining actual event logs into visual flow diagrams and quantitative journey models. Unlike traditional survey-based methods, it grounds stakeholder conversations in observed data, making requirements validation and process gap analysis more objective. Its MCP server integration means BA agents and LLM-powered workflows can invoke journey analytics directly, reducing the manual overhead of exploratory analysis. The behavioral segmentation capabilities also help BAs identify distinct user cohorts to inform prioritization and persona refinement.

## How to use it in BA Workflows
1. **Process Discovery from Event Logs** - Load application or system event logs (CSV/DataFrame) and call `rete.eventstream` to automatically reconstruct the actual user/process flow as a directed graph, revealing undocumented paths and edge cases missed in requirements documentation.
2. **Customer Journey Validation** - Compare the designed happy path against mined journeys to identify drop-off points, loops, and unexpected transitions; use these findings to update swimlane diagrams or BPMN models with real-world accuracy.
3. **Behavioral Segmentation for Personas** - Apply built-in clustering and segmentation tools to group users by their behavioral patterns, then map clusters back to existing BA personas to validate or challenge assumed archetypes with data.
4. **A/B Test and Change Impact Analysis** - Compare event log snapshots before and after a process change or release to quantify behavioral shift; present findings to stakeholders as journey graph diffs rather than raw statistics.
5. **AI-Assisted Analytics via MCP** - Connect the Retentioneering MCP server to an AI agent or LLM-powered BA workflow so that conversational queries like "show me where users abandon the onboarding flow" trigger reproducible, auditable analytics runs automatically.

## Key Features
- Event stream preprocessing with funnel and path analysis
- Graph-based user flow visualization (Sankey diagrams, transition matrices)
- Process mining models compatible with PM4Py-style analysis
- Markov chain simulation for predicting user behavior
- Built-in A/B test analytics for behavioral comparison
- MCP server for AI agent integration
- Agent skills for LLM-driven clickstream analysis

## Technology Stack
- **Languages:** Python
- **Dependencies:** pandas, numpy, plotly, scikit-learn, networkx
- **License:** Apache 2.0

## GitHub Resources
- [retentioneering/retentioneering-tools](https://github.com/retentioneering/retentioneering-tools) - Python toolkit and MCP server for reproducible clickstream and customer journey analytics

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[OpenLineage - Open Standard for Data Pipeline Lineage Tracking]]
