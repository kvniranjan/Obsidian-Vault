---
date: 2026-03-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, ai, llm, process-modeling, automation]
source: GitHub
---

# BPMN Assistant (LLM-Powered)

## What is it?
BPMN Assistant is an open-source LLM-powered tool for creating, editing, and interpreting BPMN (Business Process Model and Notation) diagrams through natural language conversation. Instead of manually dragging and dropping elements, you describe your process in plain English and the AI generates a valid BPMN diagram. Available at [github.com/jtlicardo/bpmn-assistant](https://github.com/jtlicardo/bpmn-assistant).

## Why it matters for Business Analysts
Process modeling is one of the most time-consuming BA activities. BPMN Assistant dramatically accelerates the first-draft stage of process documentation — a BA can describe a process verbally (as captured in meeting notes or interviews) and get a structured BPMN diagram instantly. It also helps non-technical stakeholders participate in process design by removing the barrier of learning BPMN syntax.

## How to use it in BA Workflows
1. **Rapid First Drafts** — Paste transcript snippets or bullet-point process descriptions; ask the assistant to generate the initial BPMN diagram.
2. **Iterative Refinement** — Request changes in natural language ("add an approval gateway after step 3", "split the swim lane for Finance and Operations").
3. **Process Interpretation** — Upload existing BPMN files and ask the assistant to explain them in plain English for stakeholder communication.
4. **Workshop Facilitation** — Use it live in discovery workshops to model processes in real time as stakeholders describe them.
5. **Handoff Documentation** — Generate BPMN XML output for import into Camunda, Activiti, or bpmn.io for further editing.

## Key Features
- Natural language to BPMN diagram generation
- Conversational editing — modify diagrams through follow-up prompts
- BPMN interpretation mode — explains existing diagrams in plain English
- Exports valid BPMN 2.0 XML compatible with standard workflow engines
- Open-source and self-hostable (bring your own LLM API key)
- Useful for rapid prototyping in requirements workshops

## GitHub Resources
- [jtlicardo/bpmn-assistant](https://github.com/jtlicardo/bpmn-assistant) — Main repository with setup and usage instructions

## Related Skills
- [[bpmn-io Web Modeler]]
- [[Featmap - User Story Mapping]]
- [[Stakeholder Analysis Framework]]
