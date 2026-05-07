---
date: 2026-05-07
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, workflow-automation, bpm, process-modeling, java, spring]
source: GitHub
---

# Activiti - Lightweight BPMN 2 Workflow and BPM Engine

## What is it?
Activiti is a lightweight, open-source Business Process Management (BPM) platform built around a high-performance BPMN 2.0 process engine for Java. It targets business people, developers, and system admins who need to model, deploy, and execute business processes. Distributed under the Apache 2.0 license with over 10,000 GitHub stars, it is one of the most widely adopted open-source BPM engines.

## Why it matters for Business Analysts
Activiti gives BAs a runtime environment to transform BPMN 2.0 process models into executable workflows without handing off to a proprietary vendor. BAs can prototype process automations directly from their diagrams and observe how process instances behave against business rules. The built-in task and form engine lets BAs design human task steps alongside automated steps, making handoff and escalation logic visible and testable. Its REST API and Spring integration mean that BA-designed processes can be embedded in existing enterprise systems with minimal developer effort.

## How to use it in BA Workflows
1. **Process Prototyping** - Model an AS-IS or TO-BE process in a BPMN 2.0 modeler (such as bpmn-js or Open-BPMN), export the `.bpmn` file, and deploy it to an Activiti engine to validate that the flow executes as intended before stakeholder sign-off.
2. **Human Task Design** - Define user task forms within BPMN diagrams to specify exactly which data fields actors must complete at each step, producing precise data requirements and handoff specifications.
3. **Business Rule Integration** - Embed service tasks that call external decision engines (e.g., Drools DMN tables) to document and enforce business rules as part of the process, creating living traceability between rules and process steps.
4. **SLA and Timer Modelling** - Use BPMN boundary timer events to encode service level agreements and escalation paths, making time-based requirements explicit and testable in a running process.
5. **Requirements Validation via Execution** - Run synthetic process instances with representative data to validate that acceptance criteria hold across happy-path, exception, and edge-case scenarios before development begins.

## Key Features
- Full BPMN 2.0 engine supporting tasks, gateways, events, sub-processes, and message flows
- REST API for process deployment, instance management, and task interaction
- Spring Boot auto-configuration for rapid embedding in microservices
- Activiti Modeler (web-based) for in-browser process design and deployment
- History service with queryable audit trail of all process and task events
- Identity and candidate group support for human task assignment and escalation
- Docker-ready deployment for quick local or cloud sandbox environments
- Activiti Cloud extension for distributed, cloud-native process execution

## Technology Stack
- **Languages:** Java (primary), JavaScript (Modeler UI)
- **Dependencies:** Spring Framework, MyBatis, Liquibase, Jackson
- **License:** Apache 2.0

## GitHub Resources
- [Activiti/Activiti](https://github.com/Activiti/Activiti) - Lightweight BPMN 2.0 workflow and BPM platform for Java with 10k+ stars

## Related Skills
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[BPMN Assistant (LLM-Powered)]]
