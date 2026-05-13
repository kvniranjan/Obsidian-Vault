---
date: 2026-05-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, dmn, process-modeling, decision-management, workflow, forms, desktop-tool]
source: GitHub
---

# Camunda Modeler - Desktop BPMN, DMN and Forms Modeling Tool

## What is it?
Camunda Modeler is a free, open-source desktop application for authoring BPMN 2.0 process diagrams, DMN 1.3 decision tables, and Camunda Forms. Built on the bpmn.io rendering libraries, it runs on Windows, macOS, and Linux and serves as the primary visual design environment for teams using the Camunda process orchestration platform. The application is MIT-licensed and installable without any subscription or account.

## Why it matters for Business Analysts
BAs can model end-to-end business processes visually with BPMN 2.0 — the universal notation understood by both business and IT — without writing any code. The built-in DMN decision table editor lets analysts capture complex business rules (eligibility criteria, pricing logic, approval thresholds) in a structured, executable format that non-technical stakeholders can review and sign off on. Token simulation lets BAs step through a process diagram like a running engine, immediately surfacing ambiguous paths and missing exception flows before any development starts. Because the modeler saves standard `.bpmn` and `.dmn` files, artefacts remain portable and can be imported into other BPMN-compliant tools or handed directly to developers for implementation.

## How to use it in BA Workflows
1. **Process Discovery Documentation** - Open a blank BPMN canvas and translate as-is or to-be process notes into a standards-compliant diagram; export to PNG/SVG for stakeholder presentations or embed `.bpmn` files directly in Confluence.
2. **Decision Rule Capture** - Use the DMN editor to convert scattered business rule documents into decision tables with clear input/output columns; share the `.dmn` file with subject-matter experts for inline review and sign-off.
3. **Process Walkthrough and Validation** - Enable the token simulation plugin, play a token through happy-path and exception flows, and record gaps; use the findings to drive requirements sign-off sessions with process owners.
4. **Requirements Handoff to Dev** - Annotate BPMN tasks with documentation text and element templates specifying service task configuration; hand the finished `.bpmn` file to developers as a living specification that the Camunda engine can execute directly.
5. **Forms Design for User Tasks** - Build Camunda Forms linked to BPMN user tasks to define required data fields and validation rules; this bridges the gap between process flow design and UI/UX requirements before front-end work begins.

## Key Features
- **BPMN 2.0 modeler** — full palette of events, gateways, tasks, subprocesses, pools, and lanes
- **DMN 1.3 decision table editor** — hit-policy selection, input/output column types, rule validation
- **Camunda Forms designer** — drag-and-drop form fields linked to process variables
- **Token simulation** — interactive, step-by-step execution walkthrough without a live engine
- **Direct deployment** — push diagrams to a running Camunda 8 SaaS or self-managed cluster from within the app
- **Element templates** — reusable connector configurations that enforce standards across process models
- **Plugin architecture** — extend with community or custom plugins (token simulation, linting, diff viewer)
- **Cross-platform desktop app** — runs on Windows, macOS, and Linux via Electron

## Technology Stack
- **Languages:** JavaScript, TypeScript
- **Runtime:** Electron (cross-platform desktop)
- **Dependencies:** bpmn.io libraries (bpmn-js, dmn-js, @bpmn-io/form-js)
- **License:** MIT

## GitHub Resources
- [camunda/camunda-modeler](https://github.com/camunda/camunda-modeler) - Free desktop application for editing BPMN, DMN, and Forms diagrams; ~1.7k stars

## Related Skills
- [[bpmn-io Web Modeler]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
