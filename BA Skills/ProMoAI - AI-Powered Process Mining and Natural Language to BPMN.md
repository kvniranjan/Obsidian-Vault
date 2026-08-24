---
date: 2026-08-24
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, process-modeling, ai-assisted-ba, data-analysis]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Natural Language to BPMN

## What is it?
ProMoAI is an AI-powered process mining suite that converts natural language descriptions and raw event logs into formal process models (BPMN or PNML). It pairs a model-generation module (ProMoAI) with an agentic analytics module (PMAx) that uses autonomous Engineer and Analyst agents to interrogate event logs and produce statistical, narrative process insights.

## Why it matters for Business Analysts
BAs are frequently asked to translate stakeholder descriptions of a process into a formal BPMN diagram, or to make sense of raw system event logs before a process-improvement initiative. ProMoAI removes the manual modeling bottleneck: a BA can describe a process in plain English and get a draft BPMN model to refine conversationally with stakeholders, or discover a baseline model directly from an event log. PMAx's agentic analytics then answers business questions about the process (bottlenecks, compliance gaps, throughput) with grounded, code-executed results rather than LLM guesses, and keeps raw event data local for privacy — useful when working with sensitive operational data.

## How to use it in BA Workflows
1. **Rapid AS-IS modeling** - Describe a process narrative from a stakeholder interview and generate a first-draft BPMN diagram to validate in the next workshop, instead of hand-drawing it.
2. **Conversational refinement** - Iterate on a generated or imported process model through natural-language chat, letting business users suggest changes without touching a modeling tool directly.
3. **Event-log-driven discovery** - Feed system event logs (e.g., ERP, ticketing, workflow engine exports) to discover the actual AS-IS process model, exposing deviations from the documented procedure.
4. **Bottleneck and compliance analysis** - Use PMAx's Analyst agent to ask business questions ("where are the delays?", "which cases violate SLA?") and get statistical visualizations plus a written narrative suitable for stakeholder reports.
5. **Privacy-conscious analytics** - Run analysis where only metadata (not raw case-level data) is sent to the LLM, making it more viable for regulated industries handling PII or financial data.

## Key Features
- Natural-language-to-BPMN/PNML generation for fast AS-IS and TO-BE modeling
- Conversational model refinement loop with business stakeholders
- Baseline process discovery directly from event logs
- Multi-agent (Engineer + Analyst) agentic analytics producing deterministic, code-executed results
- Local execution of raw event data with only metadata sent to the LLM for privacy
- Supports multiple LLM backends (OpenAI, Gemini)
- Available as a hosted app, local install, or pip-installable Python library

## Technology Stack
- **Languages:** Python (3.9+)
- **Dependencies:** Streamlit (UI), OpenAI/Gemini SDKs, process mining libraries (per requirements.txt)
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite: natural language to BPMN plus agentic event-log analytics.

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
- [[BPMN Assistant (LLM-Powered)]]
