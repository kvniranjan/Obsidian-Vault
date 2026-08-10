---
date: 2026-08-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, ai-assisted-ba, llm, process-modeling]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and BPMN Model Generation

## What is it?
ProMoAI is an open-source process mining framework that combines large language models with autonomous agents to turn natural-language descriptions, conversational refinement, or raw event logs into formal process models (BPMN or Petri nets). It also ships PMAx, an agentic analytics layer that uses specialized "Engineer" and "Analyst" agents to reason over event data and answer analytical questions in natural language.

## Why it matters for Business Analysts
BAs frequently need to turn stakeholder interviews, meeting notes, or SOP documents into formal process diagrams, and today that translation is manual and slow. ProMoAI lets a BA type a plain-English process description and get a draft BPMN model back immediately, then iteratively refine it through conversation instead of redrawing shapes in a modeling tool. Because it can also discover a baseline model directly from event logs, it bridges the "as-documented" process a BA writes with the "as-executed" process mined from systems of record. The privacy-conscious design (raw event data stays local; only metadata is sent to the LLM, and analytics are computed by generated code rather than by the LLM guessing numbers) makes it more defensible for use with sensitive operational data than a generic chatbot.

## How to use it in BA Workflows
1. **Draft-to-diagram elicitation** - After a stakeholder interview, paste a plain-language summary of the process into ProMoAI and get an initial BPMN diagram to validate with the business owner instead of drafting one from scratch.
2. **Conversational model refinement** - Iterate on a generated model by describing changes in natural language ("add a rejection branch after the credit check"), speeding up review cycles with subject-matter experts.
3. **Event-log-grounded discovery** - Feed an XES event log from a source system to generate a baseline process model, then compare it against the documented process to spot undocumented variants.
4. **Natural-language analytics with PMAx** - Ask questions about cycle time, bottlenecks, or case volume in plain English and get back agent-computed metrics instead of writing PM4Py or SQL queries directly.
5. **Rapid prototyping for requirements workshops** - Use the hosted Streamlit app live in a workshop to sketch candidate process flows on the spot as stakeholders describe them.

## Key Features
- **Text-to-model generation** - Converts natural-language process descriptions into BPMN or Petri net models
- **Conversational refinement** - Supports iterative, chat-based editing of generated models
- **Event-log discovery** - Derives baseline process models directly from XES logs
- **PMAx agentic analytics** - Divide-and-conquer Engineer/Analyst agent architecture for natural-language questions over event data
- **Privacy-aware design** - Keeps raw event data local, sending only metadata to the LLM, and computes metrics via generated code from whitelisted libraries rather than LLM guesses
- **Multi-LLM support** - Works with OpenAI, Google Gemini, and other LLM backends
- **Streamlit web interface** - Usable via a hosted demo, self-hosted app, or as an installable Python library

## Technology Stack
- **Languages:** Python (3.9+)
- **Dependencies:** Streamlit (web UI), OpenAI/Gemini SDKs, process mining libraries for BPMN/PNML/XES handling
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite converting natural language to process models via autonomous agents

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[bpmn-io Web Modeler]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
