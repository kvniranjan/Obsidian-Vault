---
date: 2026-10-08
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-mining, ai, llm, data-analysis, process-modeling]
source: GitHub
---

# ProMoAI - Generative AI Process Modeling and Agentic Process Mining

## What is it?
ProMoAI is an open-source Python suite from the fit-process-mining research group that pairs large language models with process mining. It bundles two components: ProMoAI, which generates and refines BPMN or Petri net process models from natural language, uploaded models, or event logs; and PMAx, a multi-agent "virtual process analyst" that queries event logs and produces data-grounded analytical reports.

## Why it matters for Business Analysts
ProMoAI collapses two of the most time-consuming BA activities — drafting process models and analyzing event-log data — into conversational, AI-assisted workflows. A BA can describe a process in plain English and get a reviewable BPMN diagram, or point PMAx at a real event log and receive a narrative report with tables and charts instead of writing analysis code by hand. Its privacy design (only column names and types are sent to the LLM, with deterministic metrics computed by locally-run, whitelisted Python code rather than left to LLM guesswork) makes it realistic to use on sensitive operational data, which is often a blocker for AI adoption in BA analytics work.

## How to use it in BA Workflows
1. **Rapid Process Model Drafting** - Describe a process in natural language during or after a discovery workshop and have ProMoAI generate an initial BPMN or Petri net model for review with stakeholders.
2. **Model Refinement via Chat** - Upload an existing process model (e.g., exported from bpmn-js or Camunda Modeler) and iteratively refine it through conversational follow-ups instead of manual re-editing.
3. **Discovery-then-Refine on Real Data** - Feed an XES event log to discover an as-executed model automatically, then use the LLM to clean up and annotate it for stakeholder presentation.
4. **Agentic Event-Log Analysis with PMAx** - Ask PMAx natural-language questions about an event log (bottlenecks, rework loops, SLA breaches) and receive a report with exact, code-computed metrics plus narrative insight, without writing pandas or PM4Py code.
5. **Evidence-Based Process Improvement Cases** - Combine the discovered model and PMAx's quantified findings into a single artifact to justify a process redesign recommendation to sponsors.

## Key Features
- Text-to-model generation for both BPMN and Petri net notations
- Conversational, chat-based refinement of generated or uploaded models
- Automated model discovery from XES event logs as a starting point for AI refinement
- PMAx multi-agent analytics: specialized "Engineer" and "Analyst" agents split data querying from interpretation
- Deterministic, auditable metrics — generated code runs locally against whitelisted libraries rather than relying on LLM arithmetic
- Privacy-preserving design: raw event data never leaves the local environment; only schema metadata reaches the LLM
- Usable as a hosted Streamlit app, a self-hosted app, or an installable Python library (`pip install promoai`)

## Technology Stack
- **Languages:** Python (tested on 3.9–3.10)
- **Dependencies:** Streamlit (web UI), LLM providers including OpenAI, Gemini, and GitHub Copilot models; process mining internals aligned with the PM4Py ecosystem
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - Generative AI process modeling and agentic process mining analytics suite (ProMoAI + PMAx)

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Retentioneering Tools - Process Mining and Customer Journey Analytics Toolkit]]
