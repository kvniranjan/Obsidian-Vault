---
date: 2026-04-30
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, bpm, workflow, eclipse, vscode, open-source]
source: GitHub
---

# Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web

## What is it?
Open-BPMN is a free, open-source BPMN 2.0 modeling platform built on the Eclipse Graphical Language Server Platform (GLSP). It runs natively inside Visual Studio Code, Eclipse IDE, Eclipse Theia, and as a standalone web application. Its architecture is explicitly designed to be customizable and extensible, allowing teams to tailor the editor to specific BPM workflow engines via the BPMN 2.0 extensibility mechanism.

## Why it matters for Business Analysts
BAs frequently need to create, share, and iterate on process models — often in environments where expensive commercial tools aren't available. Open-BPMN provides full BPMN 2.0 fidelity (tasks, gateways, events, lanes, subprocesses) without licensing costs, making it easy to embed process diagrams directly in developer toolchains or CI/CD pipelines. Its Java-based metamodel lets technical teams programmatically generate or parse `.bpmn` files, so BA-authored models can flow directly into execution engines like Imixs-Workflow or Camunda. Because it runs in VS Code, BAs working alongside developers can model processes in the same environment, reducing handoff friction.

## How to use it in BA Workflows
1. **As-Is / To-Be Process Modeling** - Open `.bpmn` files directly in VS Code or the web UI to draw current-state and future-state process flows using the full BPMN 2.0 palette, then share the raw XML with developers for engine execution.
2. **Requirements Traceability via Model Files** - Store `.bpmn` files in a git repository alongside requirements documents, giving every process change a tracked commit history that auditors and stakeholders can review.
3. **Handoff to Workflow Engines** - Export models produced in Open-BPMN directly to compatible engines (Imixs-Workflow, Camunda, Flowable) since the files conform to the BPMN 2.0 standard, eliminating re-drawing in engine-specific tooling.
4. **Custom Extensions for Domain Terminology** - Leverage the BPMN 2.0 extension mechanism to add domain-specific attributes (e.g., SLA fields, data classifications) to process elements, keeping business context embedded in the model itself.
5. **Embedded Diagram Reviews in IDE** - During sprint reviews or design sessions, open process diagrams inside VS Code and annotate or update them live alongside code changes, keeping process documentation in sync with implementation.

## Key Features
- Full BPMN 2.0 support: tasks, events, gateways, pools, lanes, message flows, and subprocesses
- Multi-platform: VS Code extension, Eclipse IDE plugin, Eclipse Theia, and standalone web app
- Extensible metamodel: add custom attributes and behaviors for specific workflow engines without forking
- Java BPMN 2.0 metamodel library for programmatic model generation, import, and export
- Open `.bpmn` file format — compatible with any BPMN 2.0-compliant engine
- Active development with regular releases on GitHub

## Technology Stack
- **Languages:** Java (metamodel/server), TypeScript (GLSP client/diagram editor)
- **Dependencies:** Eclipse GLSP, Eclipse Theia, VS Code Extension API, Node.js
- **License:** MIT

## GitHub Resources
- [imixs/open-bpmn](https://github.com/imixs/open-bpmn) - BPMN 2.0 modeler based on Eclipse Graphical Language Server Platform, runs in VS Code, Eclipse, Theia, and standalone web

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[dmnmd - DMN Decision Tables in Markdown]]
