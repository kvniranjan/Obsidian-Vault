---
date: 2026-10-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, workflow-automation, bpm-engine]
source: GitHub
---

# Bonita Engine - Open-Source BPMN Process Execution Engine

## What is it?
Bonita Engine is the open-source core runtime of the Bonita BPM platform, developed by Bonitasoft. It executes BPMN 2.0 process definitions, manages process instances, tasks, and business data, and exposes Java APIs for building process-driven applications. It is the execution layer behind Bonita Studio's visual process designer, letting modeled processes run as real, trackable workflows.

## Why it matters for Business Analysts
BAs frequently model "as-is" and "to-be" processes in BPMN, but value is only realized when those diagrams become executable, auditable workflows rather than static documentation. Bonita Engine closes that gap: a BA-authored BPMN diagram (built in Bonita Studio or any BPMN 2.0-compliant tool) can be deployed directly and run with real task assignments, forms, and business data. This supports process governance, SLA tracking, and continuous process improvement, since every instance's execution history becomes a dataset for later process mining and re-analysis.

## How to use it in BA Workflows
1. **Executable process modeling** - Translate discovery workshops and as-is process maps into BPMN 2.0 diagrams that can be deployed and run as live workflows, not just documentation.
2. **Task and SLA tracking** - Monitor how long tasks sit with each role or actor, surfacing bottlenecks for process improvement recommendations.
3. **Business rule and data validation** - Attach business data models and connectors to process steps, letting BAs specify validation and routing logic without engineering code changes.
4. **Stakeholder sign-off loops** - Model approval and escalation steps (multi-level sign-off, exception handling) directly in the process so stakeholder governance is enforced by the engine, not manual follow-up.
5. **Process mining feed** - Export execution logs and audit trails as a structured dataset for process mining tools (e.g., PM4Py, Cortado) to validate whether real execution matches the modeled process.

## Key Features
- Full BPMN 2.0 execution support, including gateways, events, sub-processes, and multi-instance tasks
- Java and REST APIs for integrating process execution into existing enterprise applications
- Business data model support for attaching structured data to process variables and forms
- Connector framework for integrating external systems (databases, REST/SOAP services, messaging) into process steps
- Audit trail and execution history for compliance, SLA, and process-mining analysis
- Clustering and scalability support for enterprise-grade process volumes

## Technology Stack
- **Languages:** Java
- **Dependencies:** Gradle build system, relational database (PostgreSQL/MySQL/Oracle), Bonita Studio (for visual modeling, separate component)
- **License:** GNU Lesser General Public License v2.1 (LGPL-2.1)

## GitHub Resources
- [bonitasoft/bonita-engine](https://github.com/bonitasoft/bonita-engine) - Core Java engine that executes BPMN 2.0 processes for the Bonita BPM platform

## Related Skills
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[Activiti - Lightweight BPMN 2 Workflow and BPM Engine]]
- [[Operaton - Community-Driven BPMN Process Automation Engine]]
- [[PM4Py - Process Mining for Business Analysts]]
