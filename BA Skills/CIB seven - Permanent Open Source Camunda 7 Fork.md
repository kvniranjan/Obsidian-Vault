---
date: 2026-11-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-automation, workflow, dmn, bpm, open-source, java]
source: GitHub
---

# CIB seven - Permanent Open Source Camunda 7 Fork

## What is it?
CIB seven is a fully open-source workflow and process automation framework built around a native BPMN 2.0 process engine that runs on the JVM. It is maintained by CIB as "the permanent open source Camunda 7 fork," created to give organisations a long-term, vendor-independent continuation path after Camunda 7 Community Edition reached end-of-life. It is released under the Apache License 2.0, with no open-core tiers or feature gating.

## Why it matters for Business Analysts
CIB seven preserves the full Camunda 7 BPMN/DMN modeling and execution experience BAs already know, so existing process models, decision tables, and stakeholder training carry over without rework. Its bundled web applications (Cockpit, Tasklist, Admin) let BAs inspect live process instances, manage human tasks, and administer users without writing code, closing the loop between process design and day-to-day operations. Because it is a drop-in migration target for teams leaving Camunda 7, BAs can confidently recommend it when auditing legacy BPM platforms for continued support and compliance. Its Apache 2.0 licensing (no enterprise edition required) also removes a common blocker when BAs are asked to justify tooling choices to procurement or compliance stakeholders.

## How to use it in BA Workflows
1. **Process Modeling and Deployment** - Design BPMN 2.0 diagrams with Camunda-compatible modeling tools, then deploy them directly to a CIB seven engine via REST API or the admin console to turn whiteboard diagrams into executable, auditable processes.
2. **Decision Logic Capture** - Use the bundled `engine-dmn` module to encode eligibility rules, routing logic, or approval thresholds as DMN decision tables that BAs can own and update without developer involvement.
3. **Human Task and Approval Tracking** - Use the Tasklist web app to model and demonstrate approval chains, escalations, and exception-handling paths during requirements workshops with stakeholders.
4. **Legacy Platform Migration Assessment** - When a BA is evaluating a Camunda 7 EOL migration, use CIB seven as the lowest-risk comparison baseline since it requires no changes to existing BPMN/DMN artifacts.
5. **Operational Visibility for Process Improvement** - Use the Cockpit dashboard to review running/completed process instances and incident rates, gathering the evidence base for process-optimisation recommendations.

## Key Features
- **BPMN 2.0 execution engine** - Native support for tasks, gateways, events, sub-processes, and message/signal correlation, embeddable as a Java library
- **DMN decision engine** - Execute decision tables and decision requirements graphs alongside BPMN flows via the `engine-dmn` module
- **Web apps (Cockpit / Tasklist / Admin)** - Browser UIs for process monitoring, human task management, and user/group administration out of the box
- **REST API** - Full HTTP API for deploying process definitions, starting instances, querying variables, and completing tasks
- **Spring Boot & Quarkus integration** - Embed the engine in existing Java microservices with starter modules and a Quarkus extension
- **Camunda 7 drop-in compatibility** - Direct migration path for teams moving off Camunda 7 Community Edition with no BPMN/DMN model changes
- **Enterprise adoption** - Vendor reports production use across 1,000+ companies, indicating real-world maturity beyond a hobby fork

## Technology Stack
- **Languages:** Java
- **Dependencies:** Spring Boot, Quarkus, Jakarta EE/Java EE application servers, bpmn.io tooling for modeling
- **License:** Apache License 2.0

## GitHub Resources
- [cibseven/cibseven](https://github.com/cibseven/cibseven) - CIB seven main source code repository; permanent open-source Camunda 7 fork

## Related Skills
- [[Operaton - Community-Driven BPMN Process Automation Engine]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[Fluxnova - FINOS Open-Source BPMN and DMN Process Orchestration Platform]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[Activiti - Lightweight BPMN 2 Workflow and BPM Engine]]
- [[dmn-js - Browser-Based DMN Decision Table Viewer and Editor]]
