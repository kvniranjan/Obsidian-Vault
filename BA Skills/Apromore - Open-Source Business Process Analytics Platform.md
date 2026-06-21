---
date: 2026-06-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, bpmn, process-analytics, conformance-checking, workflow-analysis, process-discovery]
source: GitHub
---

# Apromore - Open-Source Business Process Analytics Platform

## What is it?
Apromore is an open-source, online business process analytics platform that supports the full stack of process mining functionality. It enables analysts to import event logs and BPMN models, discover process maps, perform conformance checking, and analyze performance across activities and handovers. It is available as a self-hosted web application deployable via Docker.

## Why it matters for Business Analysts
Process mining bridges the gap between how processes are documented and how they actually execute — Apromore gives BAs the tooling to do this analysis without writing code. BAs can import event logs from systems like ERP or CRM, automatically discover process models, and visually compare intended vs. actual flows to identify bottlenecks, rework loops, and compliance gaps. The built-in BPMN editor means discovered models can be refined and shared directly as requirements artifacts. The no-code filtering and slicing capabilities allow BAs to segment by case variant, timeframe, or performance measures to focus stakeholder conversations on specific problem areas.

## How to use it in BA Workflows
1. **As-Is Process Discovery** - Import event logs from source systems (ERP, ticketing, CRM) and run the Process Discoverer to generate an accurate as-is process map, replacing assumptions with data-driven evidence before requirements workshops.
2. **Conformance Checking** - Compare the discovered process model against the formally documented BPMN model to identify deviations, rework, and non-compliant paths that become inputs for gap analysis and improvement requirements.
3. **Performance Bottleneck Analysis** - Overlay frequency and duration statistics on the process map to pinpoint high-wait-time handovers or high-rework activities, directly informing where process redesign will deliver the greatest value.
4. **Process Variant Analysis** - Use case-variant filtering to segment process executions by region, team, product line, or customer segment, enabling targeted stakeholder presentations with relevant evidence.
5. **BPMN Model Authoring and Sharing** - Use the integrated model editor to draft or refine BPMN process models, store them in the portal, and share them with stakeholders as collaborative, versioned artifacts.

## Key Features
- **Process Discoverer** - Automated discovery of process maps and BPMN models from event logs with frequency/duration overlays
- **BPMN Model Editor** - Full-featured editor for creating and editing process models within the platform
- **Apromore Portal** - Central repository for storing, organizing, and sharing event logs and process models with user/group access control
- **Conformance Checking** - Automated comparison of observed behavior against reference BPMN models
- **Advanced Event Log Filtering** - No-code slicing by case variant, timeframe, performance measures, execution path, rework degree, and attribute-value pairs
- **Business Calendar Manager** - Define working calendars for accurate duration calculations across time zones
- **Docker Deployment** - Containerized setup for easy self-hosted installation

## Technology Stack
- **Languages:** Java (SE 11+), JavaScript, HTML, CSS, YAML
- **Build:** Gradle
- **Database:** MySQL (production), H2 (evaluation)
- **Caching:** Ehcache
- **License:** GNU LGPL v3.0

## GitHub Resources
- [apromore/ApromoreCore](https://github.com/apromore/ApromoreCore) - Apromore Open-Source Core Edition — process mining, BPMN modeling, and analytics platform

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Cortado - Interactive Process Mining and Discovery Tool]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
