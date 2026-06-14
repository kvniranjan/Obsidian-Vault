---
date: 2026-06-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-automation, process-mining, rpa, ai-agents, llm, computer-use, workflow-automation]
source: GitHub
---

# OpenAdapt - AI-First Generative Process Automation and RPA

## What is it?
OpenAdapt is an open-source Generative RPA (Robotic Process Automation) framework that uses large language models (LLMs), large multimodal models (LMMs), and visual language models (VLMs) to record, understand, and replay user workflows on a computer. Unlike traditional RPA that relies on brittle pixel/coordinate matching, OpenAdapt captures the semantic intent of actions so that automations generalize across UI changes and edge cases. It supports multiple AI providers including OpenAI, Anthropic, Google Gemini, and HuggingFace models.

## Why it matters for Business Analysts
BAs spend significant time documenting as-is processes by shadowing users or running workshops — OpenAdapt automates this by recording real user interactions and extracting structured process knowledge from them. The AI-driven replay engine means BAs can record a workflow once and propose a working automation prototype to stakeholders without writing code, dramatically shortening the path from process discovery to proof-of-concept. Its process mining output helps BAs identify bottlenecks, deviations, and automation candidates within existing workflows. For organizations evaluating automation ROI, OpenAdapt provides concrete, replayable evidence of how processes actually run versus how they are documented to run.

## How to use it in BA Workflows
1. **As-Is Process Discovery** - Install OpenAdapt and ask a subject-matter expert to perform their normal tasks; the tool records every action, screenshot, and UI state, producing a structured event log that BAs can analyze to build accurate as-is process maps without lengthy interview cycles.
2. **Automation Prototype for Stakeholders** - After recording a process, trigger replay to generate a live automation prototype; present this to business stakeholders as a working demonstration of the proposed to-be state, accelerating buy-in and requirements sign-off.
3. **Process Documentation Generation** - Use the recorded event logs and AI-generated summaries to auto-draft SOP (Standard Operating Procedure) documents, user guides, or BPMN process descriptions — reducing manual documentation effort.
4. **Bottleneck and Deviation Analysis** - Compare multiple recordings of the same process across different users to identify deviations from the intended workflow, highlight steps where users struggle, and prioritize which pain points to address in the requirements backlog.
5. **RPA Candidate Evaluation** - Use OpenAdapt to systematically record repetitive back-office tasks (data entry, report extraction, form submission) and generate an objective complexity and feasibility assessment to support build-vs-buy or automation vendor selection decisions.

## Key Features
- **Generative Replay** - LLM/VLM models interpret recorded actions semantically, so replays adapt to minor UI changes rather than breaking on pixel shifts
- **Multi-Model Support** - Pluggable AI backends: OpenAI GPT-4o, Anthropic Claude, Google Gemini, and open-source HuggingFace models
- **Computer Use Integration** - Leverages OmniParser and Segment Anything for robust screen understanding across any application
- **Process Mining Output** - Recorded sessions produce structured event logs compatible with process mining analysis
- **Agent Framework** - Built-in AI agent orchestration (ai-agents-framework) for chaining multi-step automation tasks
- **MIT Licensed** - Fully open source; no vendor lock-in for enterprise adoption

## Technology Stack
- **Languages:** Python
- **Dependencies:** OpenAI SDK, Anthropic SDK, HuggingFace Transformers, Ultralytics (YOLO), OmniParser, Segment Anything Model (SAM)
- **License:** MIT

## GitHub Resources
- [OpenAdaptAI/OpenAdapt](https://github.com/OpenAdaptAI/OpenAdapt) - Open Source Generative Process Automation using LLMs/VLMs for AI-first RPA and process discovery

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
- [[LangGraph - AI Agent Orchestration Framework]]
- [[n8n - Fair-Code Workflow Automation Platform]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
