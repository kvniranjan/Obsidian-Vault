---
date: 2026-11-23
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, bpmn, process-mining, ai-assisted-ba, agentic-ai]
source: GitHub
---

# ProMoAI - AI-Powered Process Modeling and Agentic Process Mining Suite

## What is it?
ProMoAI is an open-source suite from Fraunhofer FIT and RWTH Aachen that uses Large Language Models to turn natural language, event logs, or existing diagrams into formal process models (BPMN or Petri nets). It now bundles PMAx, an agentic analytics module that deploys specialized "Engineer" and "Analyst" agents to answer business questions directly against event-log data and return tables, charts, and narrative reports.

## Why it matters for Business Analysts
BAs frequently need to translate stakeholder descriptions of a process into a formal diagram, or mine an existing event log to understand how a process actually runs versus how it's documented. ProMoAI lets a BA type a plain-language description of a workflow and get a reviewable BPMN diagram back, then iteratively refine it through chat rather than manual re-drawing. PMAx extends this further by letting a BA ask analytical questions ("where are the bottlenecks in this process?") and get locally-computed, LLM-narrated answers without exposing raw case data to the model — a meaningful control for BAs working with sensitive operational data.

## How to use it in BA Workflows
1. **Rapid as-is/to-be modeling** - Describe a process in plain text during a stakeholder interview and generate a draft BPMN model on the spot for validation, instead of transcribing notes into a diagramming tool after the fact.
2. **Model refinement via chat** - Upload an existing BPMN or Petri net (e.g., exported from bpmn-js or Camunda Modeler) and ask the LLM to add exception paths, rename tasks, or restructure gateways conversationally.
3. **Discovery from event logs** - Feed an XES event log to generate an initial discovered model, then have the LLM clean up and simplify the discovered structure into something stakeholder-readable.
4. **Constraint-driven discovery (POWL/DECLARE)** - Extract or author DECLARE constraints from a log, review their support/confidence, and generate a constrained process model, useful for conformance and compliance-focused BA work.
5. **Agentic process analytics (PMAx)** - Ask natural-language business questions against an event log; the Engineer/Analyst agents write and run local Python to compute exact metrics and return charts and a narrative report, supporting quick ad-hoc process analysis without a data science handoff.

## Key Features
- Text-to-model generation of BPMN or PNML diagrams from natural language descriptions.
- Chat-based refinement of uploaded BPMN/Petri net models.
- Discovery-then-refine pipeline: mine an initial model from an XES log, then let the LLM clean it up.
- Rule-based POWL discovery using DECLARE constraints with event-, trace-, or edit-distance repair.
- PMAx agentic analytics: Engineer and Analyst agents collaborate to answer business questions from event logs.
- Privacy-conscious design: only column names/types (metadata) go to the LLM; raw event data and computation stay local.
- Available as a hosted Streamlit app, a local Streamlit app, or an installable Python library (`pip install promoai`).

## Technology Stack
- **Languages:** Python (3.11+ required for POWL discovery)
- **Dependencies:** Streamlit (UI), LLM APIs (OpenAI, Gemini, and other LLM backends), process mining libraries for XES/BPMN/Petri net handling
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process modeling and agentic process mining suite combining text/log-to-BPMN generation with autonomous event-log analytics.

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Camunda - BPMN Process Orchestration Framework]]
