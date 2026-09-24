---
date: 2026-09-24
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, dmn, workflow-automation, camunda]
source: GitHub
---

# Miragon BPMN Modeler - Multi-Engine BPMN, DMN, and Camunda Forms Editor

## What is it?
Miragon BPMN Modeler is an open-source suite of editors for BPMN 2.0 process diagrams, DMN decision tables, and Camunda Forms, built on the same bpmn.io toolkit that powers the official Camunda Modeler. It ships as a VS Code extension and as a standalone Electron/Theia desktop app, with engine-aware support for Camunda 7, Camunda 8, Operaton, and CIB seven, plus planned AI-assistant integration.

## Why it matters for Business Analysts
BAs who document processes for automation teams often need to move between requirements docs and the exact BPMN/DMN artifacts developers will deploy - this tool lets them edit those artifacts directly inside a lightweight editor without standing up a full Camunda environment. The engine-aware properties panel prevents BAs from specifying process or decision logic that isn't valid for the target engine, reducing rework during handoff. Built-in visual diffing makes it easy to review what changed between process versions during requirements walkthroughs or change-control discussions. Because it is free, local-first, and works offline, it is a low-friction way for BAs to draft or refine process and decision models before developers wire them into a live deployment.

## How to use it in BA Workflows
1. **Process discovery and drafting** - Sketch BPMN 2.0 diagrams of current-state and future-state business processes directly in VS Code or the desktop app, using the same notation developers will later execute.
2. **Decision table modeling** - Use the DMN editor to formalize business rules and decision logic (e.g., approval thresholds, eligibility criteria) captured during stakeholder interviews, in a format ready for the decision engine.
3. **Form specification** - Design and preview Camunda Forms visually to specify the data-entry requirements for human tasks within a process, bridging the gap between a BA's UI/data requirements and the developer-facing form JSON.
4. **Version comparison for change requests** - Use the visual diff tool to compare two versions of a BPMN or DMN file when documenting a process change request or reviewing a proposed redesign.
5. **Engine-target validation** - Select the correct target engine (Camunda 7, Camunda 8, Operaton, CIB7) so that process/decision models a BA hands off are guaranteed compatible with what the implementation team will deploy, avoiding "that's not valid in our engine" rework.

## Key Features
- Full BPMN 2.0 and DMN modeling with engine-aware properties (no manual profile switching between Camunda 7/8 semantics)
- Visual Camunda Forms editor with linked navigation from Camunda 8 User Tasks
- Built-in visual diff tool for comparing diagram versions
- Deploy-from-editor sidebar that can push diagrams to a running Camunda 7/8 instance and start a process instance
- Element templates picked up automatically by convention from a project's `.camunda/element-templates/` folder
- Available as a VS Code extension and as a standalone Electron/Theia desktop app (no IDE required)
- Localized into 9 languages including English, German, Spanish, French, Portuguese, Russian, and Chinese variants

## Technology Stack
- **Languages:** TypeScript
- **Dependencies:** bpmn.io toolkit (bpmn-js, dmn-js), VS Code Extension API, Eclipse Theia/Electron (desktop app)
- **License:** Apache License 2.0

## GitHub Resources
- [Miragon/bpmn-modeler](https://github.com/Miragon/bpmn-modeler) - BPMN/DMN modeler and Camunda Forms editor for VS Code and desktop, supporting Camunda 7/8, Operaton, and CIB seven

## Related Skills
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[bpmn-io Web Modeler]]
- [[dmn-js - Browser-Based DMN Decision Table Viewer and Editor]]
- [[Operaton - Community-Driven BPMN Process Automation Engine]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
