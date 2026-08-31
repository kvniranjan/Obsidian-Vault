---
date: 2026-08-31
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, process-modeling, ai-assisted-ba-workflows, decision-management]
source: GitHub
---

# ProMoAI - AI-Powered Process Mining and Agentic Process Analytics

## What is it?
ProMoAI is an open-source suite that connects natural language with formal process analysis using large language models. It has two parts: the core ProMoAI tool, which turns free-text descriptions or XES event logs into formal process models (BPMN diagrams or Petri nets) and lets users refine them conversationally, and PMAx, an autonomous multi-agent system that acts as a virtual process analyst over event log data.

## Why it matters for Business Analysts
BAs are regularly asked to translate "how the process actually works" — gathered from interviews, documentation, or raw system logs — into a formal, reviewable process model, and then to answer stakeholder questions about bottlenecks and deviations. ProMoAI automates the first mile (draft a BPMN model from a narrative description or discovered event log) and the analytical mile (ask a plain-language question about the process and get back a grounded report with metrics, tables, and charts) without requiring the BA to write code or learn a process-mining library. Because PMAx computes metrics by generating and running Python locally rather than letting the LLM guess numbers, the answers stay traceable to the actual data — important when a BA has to defend a finding to stakeholders. It's a natural companion to log-based process mining and BPMN modeling tools already in a BA's kit.

## How to use it in BA Workflows
1. **Draft process models from stakeholder narratives** - Paste a written description of a process gathered during requirements interviews and let ProMoAI generate an initial BPMN diagram as a discussion starting point for validation workshops.
2. **Discover as-is models from system logs** - Feed an XES event log exported from an ERP, ticketing, or workflow system to automatically discover the actual process flow, surfacing variants stakeholders may not have described accurately.
3. **Iteratively refine models conversationally** - Use natural-language follow-up prompts to add branches, merge activities, or correct a generated model instead of manually editing BPMN XML.
4. **Ask ad-hoc analytical questions with PMAx** - Pose business questions ("where are our biggest delays?", "which cases loop back most often?") directly against event data and receive a narrative report with supporting tables and charts, useful for process-improvement business cases.
5. **Keep sensitive data local while using cloud LLMs** - Rely on PMAx's design of sending only metadata to the LLM and computing real metrics locally, which helps satisfy data-governance concerns when analyzing operational data with external AI services.

## Key Features
- Natural-language-to-BPMN/Petri-net model generation from text descriptions
- XES event log import for automated process discovery
- Conversational, iterative model refinement
- PMAx agentic analytics layer that plans, writes, and runs local Python to compute exact metrics (reduces LLM hallucination risk)
- Auto-generated narrative reports with tables and charts for stakeholder-ready insights
- Hosted demo (promoai.streamlit.app) alongside local/self-hosted installation

## Technology Stack
- **Languages:** Python (3.9–3.10)
- **Dependencies:** Streamlit (UI), OpenAI/Gemini APIs (LLM backends), BPMN/PNML/XES process-mining standards
- **License:** AGPL-3.0

## GitHub Resources
- [fit-process-mining/ProMoAI](https://github.com/fit-process-mining/ProMoAI) - AI-powered process mining suite that converts natural language to process models and uses autonomous agents to analyze event logs

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Apromore - Open-Source Business Process Analytics Platform]]
