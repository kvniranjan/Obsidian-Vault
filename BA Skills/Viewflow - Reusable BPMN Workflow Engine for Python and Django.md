---
date: 2026-07-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, workflow-automation, python, django, process-modeling, low-code]
source: GitHub
---

# Viewflow - Reusable BPMN Workflow Engine for Python and Django

## What is it?
Viewflow is a low-code library for building BPMN-driven workflow applications on top of Django. It lets you define BPMN process diagrams as Python code and execute them as live, stateful workflows. Unlike finite state machines, it natively supports parallel task execution, user task assignment, and concurrent process branches — all the constructs that appear in real BA process models.

## Why it matters for Business Analysts
BAs spend significant effort designing BPMN process models that then get handed off to developers for implementation — often with a gap between the model and the running system. Viewflow closes that gap by making the BPMN model itself the executable artifact in Python, so the BA's design directly drives the application. It handles the hard parts of workflow execution — permission checks, concurrent updates, task state transitions, and parallel gateway synchronization — letting BAs validate their process logic against real data. The open-source core is freely available under AGPL, making it accessible for internal tooling and prototypes without licensing cost.

## How to use it in BA Workflows
1. **Process Prototyping** - Translate a BPMN diagram into Viewflow's Python API to create a running prototype of a business process, enabling early validation of flow logic before full development begins.
2. **Human Task Management** - Model approval chains, review loops, and multi-role handoffs using Viewflow's user task and inbox components to demonstrate how work will move between stakeholders.
3. **Parallel Process Validation** - Use BPMN parallel gateways in Viewflow to test concurrent-execution scenarios (e.g. simultaneous approvals) and confirm the process handles race conditions correctly.
4. **Requirements Demonstration** - Run a live Django app from the workflow model to give stakeholders a clickable demo of the to-be process without building a full production system.
5. **Integration Baseline** - Use Viewflow's Django integration to connect workflow steps to real database models and forms, producing a functional baseline that developers can extend rather than rewrite from scratch.

## Key Features
- BPMN 2.0 workflows written as Python classes — no separate XML tooling required
- Parallel gateway support for concurrent branches and synchronization points
- Built-in user inbox, task state tracking, and permission enforcement
- Django admin and SPA-style frontend for process monitoring out of the box
- CRUD and form generation utilities for building data-entry tasks alongside workflow steps
- Open-source core (AGPL) with a commercial PRO edition for advanced features and third-party integrations

## Technology Stack
- **Languages:** Python, JavaScript
- **Dependencies:** Django, Django REST Framework (for API flows)
- **License:** AGPL-3.0 (core); commercial for Viewflow PRO

## GitHub Resources
- [viewflow/viewflow](https://github.com/viewflow/viewflow) - Reusable BPMN workflow library for Django

## Related Skills
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Activiti - Lightweight BPMN 2 Workflow and BPM Engine]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Operaton - Community-Driven BPMN Process Automation Engine]]
- [[bpmn-io Web Modeler]]
- [[n8n - Fair-Code Workflow Automation Platform]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
