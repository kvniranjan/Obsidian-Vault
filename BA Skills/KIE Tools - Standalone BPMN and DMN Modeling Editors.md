---
date: 2026-10-18
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, dmn, process-modeling, decision-management, vscode-extension]
source: GitHub
---

# KIE Tools - Standalone and Embeddable BPMN/DMN Editors

## What is it?
Apache KIE Tools (`incubator-kie-tools`) is a monorepo of lightweight editors for BPMN process diagrams and DMN decision tables, distributed as a VS Code extension, a Chrome extension, standalone web editors, and the browser-based KIE Sandbox. It lets anyone create, open, or edit BPMN/DMN files without installing or running a full business process engine.

## Why it matters for Business Analysts
BAs frequently need to draft or review process flows and decision logic quickly, without spinning up server infrastructure. These editors run directly in VS Code or Chrome, or as a shareable browser link, making process and decision modeling accessible to analysts who work in lightweight, file-based or git-based workflows. Because outputs are standard BPMN 2.0 and DMN XML, diagrams and decision tables created here are portable to full execution engines later, keeping analysis-stage modeling decoupled from engineering's choice of runtime.

## How to use it in BA Workflows
1. **Author BPMN diagrams in VS Code** - Install the VS Code extension to sketch as-is/to-be process flows directly alongside requirements documents in the same repository.
2. **Build DMN decision tables** - Use the DMN editor to define business rules and decision logic for use cases involving conditional policy, then hand the DMN file to engineering for execution in Drools/Kogito or another DMN-compliant engine.
3. **Quick review in Chrome** - Use the Chrome extension to open a `.bpmn` or `.dmn` file a colleague shared, and review it without any local installation.
4. **Browser-based stakeholder review via KIE Sandbox** - Share a hosted link to a process or decision model so stakeholders can review and comment without installing software.
5. **Version-controlled process documentation** - Store BPMN/DMN files in the same git repository as requirements docs, giving a diffable, auditable history of process and decision changes over time.

## Key Features
- Standalone BPMN and DMN editors that run without any backend service
- VS Code extension for editing BPMN, DMN, SceSim, and PMML files inline with other project files
- Chrome extension for no-install viewing/editing directly in the browser
- KIE Sandbox online editor with GitHub integration for sharing and reviewing models
- Fully standards-compliant BPMN 2.0 / DMN XML output, portable to Camunda, Flowable, jBPM, Operaton, and other engines

## Technology Stack
- **Languages:** TypeScript/JavaScript, Java, Go
- **Dependencies:** Node.js, pnpm, Webpack, Maven, Docker/Podman, Playwright (testing)
- **License:** Apache-2.0

## GitHub Resources
- [apache/incubator-kie-tools](https://github.com/apache/incubator-kie-tools) - Standalone and embeddable BPMN/DMN editors for VS Code, Chrome, and the browser

## Related Skills
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[dmn-js - Browser-Based DMN Decision Table Viewer and Editor]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
