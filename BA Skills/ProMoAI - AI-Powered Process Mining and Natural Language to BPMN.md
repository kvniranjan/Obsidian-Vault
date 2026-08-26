---
date: 2026-08-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, ai-assisted-ba, process-modeling]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Natural Language to BPMN

## What is it?
ProMoAI is an AI-driven process mining suite that uses Large Language Models to bridge natural language and formal process analysis. It generates BPMN diagrams and Petri nets directly from text descriptions or raw event logs, and ships with PMAx, an autonomous multi-agent system that analyzes event logs and produces business insights without manual query-writing.

## Why it matters for Business Analysts
BAs are frequently handed raw system logs or verbal process descriptions and asked to produce an AS-IS process model quickly — ProMoAI collapses that translation step by turning either input into a reviewable BPMN diagram in minutes. Its conversational refinement loop lets a BA iterate on a generated model in plain English instead of learning modeling-tool mechanics, and PMAx's autonomous analytics surfaces bottlenecks, deviations, and improvement opportunities that would otherwise require a data analyst. Because only column metadata (not raw event data) is sent to the LLM, it also fits BA workflows that touch sensitive operational data under governance constraints.

## How to use it in BA Workflows
1. **AS-IS Process Discovery** - Feed an XES/CSV event log into ProMoAI to auto-generate a BPMN or Petri net diagram of the actual process, replacing manual "walk the process" interviews with a data-backed starting draft.
2. **Rapid Process Drafting from Interviews** - Type a natural-language description captured during a stakeholder workshop and get an initial BPMN model to validate in the next review session, speeding up requirements-to-model turnaround.
3. **Conversational Model Refinement** - Use follow-up prompts ("add a rejection branch after the approval step") to iteratively correct a generated model instead of manually rewiring shapes in a modeling tool.
4. **Bottleneck and Deviation Analysis** - Run PMAx against event logs to autonomously identify slow steps, rework loops, and conformance deviations, giving BAs data-driven talking points for process improvement recommendations.
5. **Privacy-Constrained Process Analysis** - Apply it to regulated or sensitive process data since only lightweight metadata is shared with the LLM while raw event data and computation stay local.

## Key Features
- LLM-driven generation of BPMN diagrams and Petri nets from text or event logs
- Conversational model refinement without manual diagram editing
- PMAx: autonomous multi-agent analytics for event logs
- Local execution of Python code for metric computation, reducing LLM hallucination risk
- Privacy-focused design — raw event data never leaves the local environment
- Usable as a Streamlit web app or a local Python library

## Technology Stack
- **Languages:** Python 3.9/3.10
- **Dependencies:** Streamlit, LLM APIs (OpenAI, Google Gemini), BPMN/PNML/XES process-mining libraries
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite for natural-language-to-BPMN generation and autonomous event log analysis

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
