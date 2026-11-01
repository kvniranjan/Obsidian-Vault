---
date: 2026-11-01
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, llm, agentic-ai, process-modeling]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and BPMN Model Generation

## What is it?
ProMoAI is an open-source, LLM-powered suite that bridges natural language and process analysis. It has two modules: ProMoAI, which generates BPMN or Petri net (PNML) process models from plain-text descriptions or discovers them from XES event logs, and PMAx, a multi-agent "virtual process analyst" that answers business questions about event logs with data-grounded reports, tables, and charts.

## Why it matters for Business Analysts
Business analysts routinely spend hours manually translating stakeholder interviews or event logs into formal process diagrams, and then more time digging through event data to answer ad-hoc process-performance questions. ProMoAI automates both ends of that workflow: analysts can describe a process conversationally and get a reviewable BPMN diagram, or point it at a real event log and have a model discovered and then chat-refined. PMAx's "Engineer and Analyst" agent pair runs exact Python computations locally rather than letting the LLM guess metrics, so the numeric answers behind process-improvement recommendations stay trustworthy. A privacy-conscious design (only column names/types are sent to the LLM, raw event data stays local) also makes it easier to justify using in regulated or sensitive business environments.

## How to use it in BA Workflows
1. **Text-to-model generation** - Describe a business process in plain language (e.g., "an order is received, then checked for stock, then either shipped or backordered") and get a draft BPMN diagram to validate with stakeholders instead of drawing it from scratch.
2. **Event-log-driven process discovery** - Upload an XES event log from a workflow or ERP system to automatically discover the as-is process model, then use chat to clean up noise or merge near-duplicate paths.
3. **Conversational model refinement** - Upload an existing BPMN or Petri net model and iteratively refine activities, gateways, and flows through natural-language chat instead of manual diagram editing.
4. **Agentic process analytics (PMAx)** - Ask high-level business questions ("where are our bottlenecks?", "which cases take longest and why?") and receive a report combining computed metrics, charts, and narrative insight, useful for process-improvement business cases.
5. **Data-grounded decision support** - Rely on PMAx's locally executed metric calculations (rather than LLM estimation) when presenting quantitative findings to stakeholders, reducing the risk of AI-hallucinated numbers in BA deliverables.

## Key Features
- Text-to-BPMN/PNML model generation from natural language
- Automated process discovery from XES event logs with LLM-assisted refinement
- Chat-based iterative model editing
- Divide-and-conquer multi-agent analytics (Engineer agent + Analyst agent) for autonomous process Q&A
- Privacy-preserving design: only schema metadata reaches the LLM, raw event data stays local
- Exact metric computation via locally executed Python code instead of LLM-estimated numbers
- Usable as a hosted Streamlit app or installed locally as a Python library

## Technology Stack
- **Languages:** Python 3.9 / 3.10
- **Dependencies:** Streamlit (UI), process-mining libraries for XES/BPMN/PNML handling, LLM API integration; listed in `requirements.txt` and `packages.txt`; installable via `pip install promoai`
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite converting natural language to process models and using autonomous agents to analyze event logs and generate actionable process insights.

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Retentioneering Tools - Process Mining and Customer Journey Analytics Toolkit]]
