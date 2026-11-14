---
date: 2026-11-14
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, bpmn, process-mining, ai-assisted-ba, data-analysis, decision-management]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Natural Language to BPMN Generation

## What is it?
ProMoAI is an AI-powered process mining suite that bridges natural language and formal process analysis using Large Language Models (LLMs). It combines two modules: a model-generation engine that converts plain-text descriptions or event logs into BPMN/Petri net models, and PMAx, a multi-agent "virtual process analyst" that autonomously queries event logs to produce data-grounded reports and insights.

## Why it matters for Business Analysts
ProMoAI removes the steepest barrier in process modeling and process mining — needing specialized notation skills or scripting knowledge to turn stakeholder input or raw event data into a usable model. A BA can describe a process conversationally and get a reviewable BPMN diagram, or point the tool at an event log and receive a discovered model refined through further chat. The PMAx analytics agent lets a BA ask high-level business questions in plain language and get back tables, charts, and narrative insights, while keeping raw event data local and only sending lightweight metadata to the LLM — a meaningful consideration for BAs handling sensitive operational data.

## How to use it in BA Workflows
1. **Rapid process documentation** - Describe a business process in natural language during or after a stakeholder interview and generate an initial BPMN diagram to validate understanding before formal documentation.
2. **As-is process discovery from logs** - Feed an XES event log from a workflow or ERP system to discover the actual as-is process model, then refine it through chat to clarify exceptions or rare paths.
3. **Constraint-based process validation** - Extract DECLARE constraints (business rules like "activity A must always precede activity B") from a process description, review their support/confidence against real data, and generate a model that respects them — useful for compliance or audit-driven process checks.
4. **Model refinement and iteration** - Upload an existing BPMN or Petri net from another tool and extend or modify it conversationally instead of manually editing nodes and connectors.
5. **Autonomous process Q&A and reporting** - Pose a business question (e.g. "where are the bottlenecks in our approval process?") and let the PMAx Engineer/Analyst agents query the event log and return deterministic, data-grounded tables, charts, and narrative summaries for stakeholder reporting.

## Key Features
- **Text-to-model generation** - Produces BPMN or PNML (Petri net) models directly from natural language process descriptions.
- **Event log discovery baseline** - Discovers an initial model from an XES log before LLM-based refinement, anchoring the model in real data.
- **Rule-based POWL discovery** - Extracts and validates DECLARE constraints, then generates a constrained process model.
- **Multi-agent analytics (PMAx)** - Engineer and Analyst agents divide reasoning work to answer open-ended business questions about process data.
- **Privacy-preserving design** - Only column names/types (not raw event data) are sent to the LLM; metrics are computed locally and deterministically rather than estimated by the model.
- **LLM-agnostic** - Supports multiple LLM backends including OpenAI and Gemini.

## Technology Stack
- **Languages:** Python (3.11+, required for POWL support)
- **Dependencies:** Streamlit (web app interface), LLM APIs (OpenAI, Gemini), installable as a library via `pip install promoai`
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite: natural language/event logs to BPMN, plus autonomous agentic analytics on event logs.

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
