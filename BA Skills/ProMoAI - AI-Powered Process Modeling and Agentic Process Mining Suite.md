---
date: 2026-08-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, bpmn, process-mining, ai-assisted-ba, decision-management]
source: GitHub
---

# ProMoAI - AI-Powered Process Modeling and Agentic Process Mining Suite

## What is it?
ProMoAI is an open-source, research-backed suite (IJCAI 2024) that uses Large Language Models to convert natural-language process descriptions into formal process models (BPMN or Petri nets), and pairs that with PMAx, an autonomous multi-agent framework that acts as a virtual process analyst over event logs. It combines generative process modeling with agentic process mining in a single Python toolkit, accessible via a hosted Streamlit app, a local Streamlit instance, or a pip-installable library.

## Why it matters for Business Analysts
BAs spend significant time translating stakeholder narratives into formal process diagrams and then interrogating event data to find bottlenecks — both are traditionally slow, manual, and require specialist tooling. ProMoAI lets a BA describe a process conversationally and get a reviewable BPMN diagram back in seconds, then refine it through chat rather than re-drawing shapes. Its PMAx analyst agent can answer plain-language questions about process performance (throughput, bottlenecks, deviations) directly from event logs, giving BAs a data-grounded second opinion without needing to write process-mining code themselves. Its privacy-preserving design — sending only metadata to the LLM while keeping raw event data local and executing deterministic Python for metrics — makes it viable for BAs working with sensitive operational or customer data.

## How to use it in BA Workflows
1. **Rapid process discovery from interviews** - Paste stakeholder interview notes or a written process description into the text-to-model interface to get a draft BPMN diagram, then iterate with follow-up chat prompts instead of manually redrawing the model.
2. **As-is process validation against event logs** - Feed an event log (CSV/XES) to PMAx and ask natural-language questions ("where are the biggest delays between order approval and shipment?") to validate or challenge the as-is model a BA has drafted.
3. **Stakeholder workshops and rapid prototyping** - Use the hosted Streamlit app live in a workshop to turn a stakeholder's spoken description of a process into a visual model on the spot, accelerating requirements elicitation sessions.
4. **Decision-point and bottleneck analysis** - Leverage the Engineer/Analyst agent pair to compute exact process metrics (cycle time, rework rate, variant frequency) grounded in real data rather than LLM guesses, supporting evidence-based process improvement recommendations.
5. **Model export for downstream BPMN tooling** - Export generated BPMN/Petri net models for further refinement in dedicated modelers (e.g. bpmn-js, Camunda Modeler) already tracked in this vault, using ProMoAI as the fast first-draft generator.

## Key Features
- Text-to-Model generation producing BPMN or Petri net formats from natural language
- Interactive chat-based model refinement, avoiding manual re-drawing for each change
- PMAx autonomous multi-agent framework with specialized Engineer and Analyst agent roles
- Privacy-preserving architecture — only lightweight metadata (column names/types) reaches the LLM, raw event data stays local
- Deterministic, code-executed metric computation rather than LLM-hallucinated statistics
- Available as a hosted app, local Streamlit deployment, or installable Python library (`pip install promoai`)

## Technology Stack
- **Languages:** Python
- **Dependencies:** Streamlit, LLM API access (via requirements.txt/packages.txt), process-mining libraries for BPMN/Petri net generation
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered suite converting natural language into BPMN/Petri net process models with autonomous agentic analysis of event logs

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
