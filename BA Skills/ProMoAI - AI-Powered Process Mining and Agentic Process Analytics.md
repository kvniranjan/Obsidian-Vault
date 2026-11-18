---
date: 2026-11-18
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, ai-assisted, data-analysis, python]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Agentic Process Analytics

## What is it?
ProMoAI is an open-source Python suite that combines large language models with classical process mining. Its model-generation module turns natural language descriptions, or raw XES event logs, into BPMN diagrams and Petri nets, and lets you refine a model conversationally through chat. Its companion module, PMAx, runs a multi-agent "Engineer + Analyst" pipeline that answers business questions about an event log and returns tables, charts, and narrative reports, generating and executing the underlying Python locally rather than guessing at numbers.

## Why it matters for Business Analysts
Process mining normally requires scripting skills BAs may not have; ProMoAI lets a BA describe a process in plain English, or point it at an exported event log, and get a reviewable BPMN model back in minutes. The conversational refinement loop turns process modeling into a dialogue instead of a diagramming exercise, which is useful for rapid workshop capture and stakeholder validation. PMAx extends this to analysis: a BA can ask "where are the bottlenecks in this fulfillment process?" and get a data-backed chart and written explanation, without writing pandas code. Because PMAx keeps raw event data local and only sends lightweight metadata (column names/types) to the LLM, it fits governance-conscious environments where process data can't leave the organization.

## How to use it in BA Workflows
1. **Draft a BPMN from a process narrative** - Describe a process in natural language (e.g., stakeholder interview notes or a SOP) and have ProMoAI generate a first-pass BPMN or Petri net model, skipping the manual drag-and-drop modeling step.
2. **Discover the as-is process from system logs** - Export an XES or CSV event log from the source system (ERP, ticketing, CRM) and run automated process discovery to see how the process actually executes, then compare it to the documented as-is model.
3. **Refine models through chat** - Iterate on a generated model conversationally ("add a rejection branch after the approval gateway") instead of re-editing shapes in a modeler, speeding up workshop-driven model revisions.
4. **Apply rule-based discovery from DECLARE constraints** - Encode known business rules as DECLARE constraints and generate a POWL model that respects them, useful when a BA already knows constraints but not the full flow.
5. **Run agentic analytics on event logs with PMAx** - Ask free-text business questions about a log ("which case variant has the longest cycle time?") and get back a chart, a table, and a plain-language explanation for a stakeholder deck, without needing a data analyst to build the query.

## Key Features
- **Text-to-BPMN/Petri net generation** - Converts natural language process descriptions into formal process models
- **Chat-based model refinement** - Incrementally edits a generated model through conversational prompts
- **Automated process discovery** - Mines BPMN/Petri net models directly from XES event logs
- **DECLARE-constrained POWL discovery** - Produces rule-compliant process models from declarative constraints
- **PMAx multi-agent analytics** - Engineer and Analyst agents collaborate to answer business questions with generated, locally-executed code
- **Privacy-conscious analysis** - Sends only log metadata to the LLM; raw event data and computation stay local
- **Multi-LLM support** - Works with OpenAI, Gemini, and other LLM backends
- **Streamlit web app** - Usable via a hosted or self-run browser UI, no coding required for basic use

## Technology Stack
- **Languages:** Python (3.11+ for POWL discovery)
- **Dependencies:** Streamlit, pm4py-family process mining libraries, OpenAI/Gemini LLM SDKs
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite for text-to-BPMN generation, event log discovery, and agentic analytics

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
- [[Retentioneering Tools - Process Mining and Customer Journey Analytics Toolkit]]
