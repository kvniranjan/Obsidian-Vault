---
date: 2026-06-30
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, dmn, workflow-automation, process-modeling, decision-management, process-orchestration, open-source, finos]
source: GitHub
---

# Fluxnova - FINOS Open-Source BPMN and DMN Process Orchestration Platform

## What is it?
Fluxnova is an enterprise-grade open-source Business Process Management (BPM) platform launched in November 2025 under the FINOS (Fintech Open Source Foundation) / Linux Foundation umbrella. It provides a complete workflow and process orchestration stack built around the BPMN 2.0 and DMN standards, with a native Java execution engine, REST API, visual process modeler, and task management interface. The project is maintained by engineering teams from Fidelity Investments, NatWest Group, Deutsche Bank, BMO, and Capital One.

## Why it matters for Business Analysts
Fluxnova gives BAs a vendor-neutral, industry-backed platform to model, execute, and monitor business processes using the BPMN and DMN standards they already know — without lock-in to proprietary tools. The visual Fluxnova Modeler (built on bpmn.io) lets BAs design process flows, decision tables, and forms in a single integrated environment that developers can deploy directly to the engine. Because the platform is backed by multiple global financial institutions as a collaborative FINOS project, its feature roadmap reflects real enterprise process automation needs: human-in-the-loop tasks, SLA tracking, process versioning, and live instance migration. BAs working in regulated or financial-services environments benefit especially from its open governance, auditability, and active 2.0/3.0 roadmap.

## How to use it in BA Workflows
1. **Process Discovery and Documentation** - Use the Fluxnova Modeler desktop app to capture as-is business processes in BPMN 2.0 notation, building a shared visual language between business stakeholders and development teams that removes ambiguity from requirements.
2. **Decision Table Design** - Model business rules using the integrated DMN decision table editor; define decision logic (eligibility criteria, pricing rules, escalation thresholds) that can be executed directly by the engine, reducing the gap between documented rules and deployed behaviour.
3. **Prototype and Validate To-Be Processes** - Deploy modeled processes to the Fluxnova Engine in a test environment and simulate execution paths, catching requirement gaps and edge cases before development investment is made.
4. **Human Task and Approval Workflow Specification** - Use the built-in human-in-the-loop and task assignment capabilities to formally specify approval chains, review steps, and escalation paths, generating executable process specs that replace lengthy narrative documents.
5. **SLA and Process Monitoring** - Leverage the engine's process visibility features to track where work sits across active instances, monitor SLA compliance, and provide stakeholders with live operational dashboards — turning BA process models into production observability artifacts.

## Key Features
- **BPMN 2.0 Engine** - Native Java execution engine for BPMN process models; embeddable in any JVM application
- **DMN Decision Engine** - Execute decision tables and decision requirement diagrams alongside process flows
- **Fluxnova Modeler** - Integrated desktop application for BPMN, DMN, and Forms design based on the bpmn.io library
- **Fluxnova Tasklist** - Web application for managing and completing human tasks within running processes
- **REST API** - Full remote API for integration with existing systems and frontend applications
- **Process Versioning** - Deploy new process versions and migrate live instances without disruption
- **Human-in-the-Loop** - Built-in task assignment, escalation, timeout, and manual intervention capabilities
- **Active Roadmap** - Versions 2.0 and 3.0 already planned, with an active FINOS community and enterprise backers

## Technology Stack
- **Languages:** Java (engine), JavaScript/TypeScript (modeler, tasklist)
- **Dependencies:** JVM runtime; bpmn.io for modeler; Spring Framework compatible
- **License:** Apache 2.0

## GitHub Resources
- [finos/fluxnova-bpm-platform](https://github.com/finos/fluxnova-bpm-platform) - Core BPM platform: engine, REST API, and deployment infrastructure
- [finos/fluxnova-modeler](https://github.com/finos/fluxnova-modeler) - Integrated BPMN, DMN, and Forms modeling desktop application

## Related Skills
- [[Camunda - BPMN Process Orchestration Framework]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[Operaton - Community-Driven BPMN Process Automation Engine]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[dmn-js - Browser-Based DMN Decision Table Viewer and Editor]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
