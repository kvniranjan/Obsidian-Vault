---
date: 2026-11-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, diagramming, process-modeling, bpmn, flowcharts, requirements-management]
source: GitHub
---

# draw.io - Free Open-Source Diagramming Editor for Process and System Modeling

## What is it?
draw.io (jgraph/drawio) is a free, open-source, client-side diagramming editor built in JavaScript that runs entirely in the browser, as a desktop app, or embedded in other tools (Confluence, Jira, VS Code, GitHub, Google Drive). It ships with a library of over 10,000 shapes — including flowchart, BPMN, UML, ER, network, and AWS/Azure/GCP architecture stencils — and stores diagrams as portable, versionable XML.

## Why it matters for Business Analysts
draw.io is the de facto free tool BAs reach for when they need a process flow, swimlane diagram, org chart, wireframe, or data model without licensing a commercial tool like Visio or Lucidchart. Because it runs client-side with no account or server required, diagrams can be created and shared instantly during a workshop, embedded directly in Confluence/Jira tickets for requirements traceability, or stored as plain XML in a git repo alongside specs for version control and diffing. Its wide shape library covers nearly every notation a BA needs — BPMN swimlanes, flowcharts, ERDs, C4/architecture diagrams — in a single tool, and its open file format means diagrams aren't locked into a proprietary vendor.

## How to use it in BA Workflows
1. **Process Flow Documentation** - Draw AS-IS/TO-BE business process flows and swimlane diagrams during or immediately after stakeholder workshops, using built-in flowchart and BPMN shape libraries.
2. **Requirements Traceability in Confluence/Jira** - Embed live-editable draw.io diagrams directly inside Confluence pages or Jira tickets so process diagrams stay next to the requirements they illustrate and update in place.
3. **Data Model and ERD Sketching** - Use the entity-relationship shape set to model data requirements collaboratively with technical teams before handoff to developers.
4. **Wireframing and UI Mockups** - Produce quick low-fidelity wireframes for discussing screen flows and UX requirements with stakeholders, without needing a dedicated design tool.
5. **Version-Controlled Diagrams-as-Documentation** - Store `.drawio` XML files in the same git repository as specs, enabling diff-based review of process changes over time alongside text requirements.

## Key Features
- **10,000+ built-in shapes** — flowchart, BPMN, UML, ER, network, and cloud architecture (AWS/Azure/GCP) stencils in one library
- **No account or server required** — fully client-side, works offline, and data never leaves the browser unless explicitly saved/exported
- **Multiple deployment modes** — web app, Electron desktop app, VS Code extension, and embeddable integrations for Confluence, Jira, and GitHub
- **Open, portable file format** — diagrams save as readable XML, enabling version control and programmatic generation/editing
- **Export flexibility** — PNG, SVG, PDF, and editable XML for sharing with both technical and non-technical stakeholders

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** mxGraph (the underlying diagramming library); Electron for the desktop build
- **License:** Apache-2.0

## GitHub Resources
- [jgraph/drawio](https://github.com/jgraph/drawio) - Free, client-side diagramming application built on mxGraph

## Related Skills
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
