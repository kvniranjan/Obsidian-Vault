---
date: 2026-11-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, process-modeling, bpmn, ai-assisted, data-analysis, python]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Natural Language Process Modeling

## What is it?
ProMoAI is an open-source Python suite that uses large language models to connect natural-language input with formal process analysis. It bundles two modules: ProMoAI for generating and refining BPMN/Petri net process models from plain text or event logs, and PMAx, an agentic "virtual process analyst" that answers business questions over event logs and produces data-grounded reports.

## Why it matters for Business Analysts
BAs are frequently asked to turn a stakeholder's description of "how the process works" into a formal diagram, or to turn raw event data into insights a stakeholder can act on — both steps are usually slow and manual. ProMoAI lets a BA describe a process in plain English and get a reviewable BPMN model back, or upload an existing model and revise it conversationally instead of re-drawing it. PMAx goes further by acting as an analyst over event logs: it answers natural-language business questions and returns tables, charts, and narrative findings with exact, locally computed numbers rather than LLM-guessed figures — which matters for stakeholder trust. Because only column names and types (not raw data) are sent to the LLM, it fits data-sensitive BA engagements better than naive "paste your data into ChatGPT" workflows.

## How to use it in BA Workflows
1. **Draft process models from stakeholder interviews** - After a requirements workshop, type up the described process in natural language and generate a first-pass BPMN diagram for stakeholders to validate, instead of manually drawing it in a modeling tool.
2. **Refine existing BPMN/Petri net models conversationally** - Upload a process model exported from another tool and ask for changes ("add an approval step before payment release") instead of hand-editing the diagram.
3. **Discover a baseline model from system logs, then clean it up with AI** - Feed an XES/CSV event log from an ERP, CRM, or ticketing system to get an auto-discovered model, then use natural language to simplify or correct it for presentation.
4. **Ask business questions directly against event logs (PMAx)** - Pose questions like "where are the biggest delays in the approval process?" and get a report with charts and a written explanation, grounded in deterministic computation rather than hallucinated numbers.
5. **Produce stakeholder-ready analysis artifacts** - Use PMAx's generated tables, statistical charts, and narrative summaries directly in process improvement decks or business cases, reducing the manual reporting step after a process mining exercise.

## Key Features
- **Text-to-model generation** - Produces BPMN or PNML models directly from natural-language process descriptions
- **Conversational model refinement** - Modify or extend an uploaded BPMN/Petri net model through chat instead of manual editing
- **Discovery baseline** - Mines an initial process model from an XES event log that the LLM can then refine
- **Agentic analytics (PMAx)** - A two-agent (Engineer + Analyst) pipeline that prepares data, computes exact metrics with local Python code, and interprets the results into a readable report
- **Privacy-conscious design** - Only metadata (column names/types) is sent to the LLM; raw event data stays local
- **Deterministic computation** - Metrics are computed by whitelisted local code rather than estimated by the LLM, avoiding hallucinated statistics

## Technology Stack
- **Languages:** Python (3.9/3.10), Streamlit for the UI
- **Dependencies:** LLM API access (model-agnostic; configured by the user), standard process mining/data libraries listed in `requirements.txt`
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite combining natural-language-to-BPMN modeling with an agentic event-log analyst

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
