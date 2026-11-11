---
date: 2026-11-11
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, ai-assisted-ba, llm, agentic-ai, data-analysis]
source: GitHub
---

# ProMoAI - AI-Powered Process Modeling and Mining Suite

## What is it?
ProMoAI is an open-source process mining suite from Fraunhofer FIT and RWTH Aachen that uses large language models to turn natural-language descriptions or raw event logs into formal process models. It can generate BPMN diagrams or Petri nets from plain text, let users refine an existing model through chat-style feedback, and run an agentic module (PMAx) that analyzes event logs to surface process insights automatically.

## Why it matters for Business Analysts
BAs routinely translate stakeholder narratives and operational event data into process diagrams that development and operations teams can act on — work that is slow and error-prone when done by hand. ProMoAI automates the first draft of that translation, letting a BA describe a process in plain English (or upload an event log) and get back a reviewable BPMN model instead of starting from a blank canvas. The chat-based refinement loop also means a BA can iterate on a model with stakeholders in near real time during a workshop, and the event-log analysis module gives BAs a way to validate "as-is" process documentation against what actually happened in the systems of record.

## How to use it in BA Workflows
1. **Rapid as-is/to-be modeling** - Paste a stakeholder's written process description or meeting transcript and generate a first-draft BPMN or Petri net model to react to rather than draft from scratch.
2. **Model refinement via feedback** - Upload an existing semi-structured BPMN/Petri net model and iteratively correct it with natural-language feedback, speeding up review cycles with process owners.
3. **Event-log-driven process discovery** - Feed exported event logs (e.g., from an ERP, ticketing, or workflow system) into the PMAx agentic module to discover the real process flow and compare it against the documented process.
4. **Process insight generation** - Use the autonomous agent analysis to flag bottlenecks, deviations, or inefficiencies in a process directly from log data, supporting data-backed process improvement recommendations.
5. **Workshop facilitation aid** - Run the hosted Streamlit app live in stakeholder workshops to visualize process changes immediately as requirements are discussed.

## Key Features
- Natural-language-to-BPMN/Petri-net generation using LLMs (supports OpenAI, Gemini, and other providers)
- POWL (partially ordered workflow language) intermediate representation ensures generated models are structurally sound before export
- Chat-based iterative model refinement from user feedback
- PMAx agentic module for autonomous event-log analysis and insight generation
- Hosted Streamlit demo app for no-install experimentation
- Exports to standard BPMN and PNML formats for use in other modeling tools

## Technology Stack
- **Languages:** Python
- **Dependencies:** LLM APIs (OpenAI, Gemini, and compatible copilots), Streamlit, PM4Py-family process mining libraries
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite that converts natural language to process models and uses autonomous agents to analyze event logs and generate actionable process insights.

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
