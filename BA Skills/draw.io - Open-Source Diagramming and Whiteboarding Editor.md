---
date: 2026-10-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, diagramming, process-modeling, bpmn, whiteboarding, github]
source: GitHub
---

# draw.io - Open-Source Diagramming and Whiteboarding Editor

## What is it?
draw.io (jgraph/drawio) is a free, open-source, client-side JavaScript diagramming and whiteboarding application. It runs entirely in the browser (or as a desktop app, Docker container, or embedded widget) with no account or server required, and ships with large stencil libraries for flowcharts, BPMN, UML, ER diagrams, network diagrams, mockups, and org charts.

## Why it matters for Business Analysts
draw.io is one of the most widely used free tools for turning a process conversation into a shareable diagram, whether that's an as-is/to-be swimlane flow, a stakeholder org chart, a wireframe for a requirement walkthrough, or an entity-relationship diagram for a data requirement. Because it is self-hosted and client-side, BAs working in regulated or security-conscious environments can diagram sensitive processes without sending data to a third-party SaaS tool. Its native integration into Confluence, Jira, GitHub, and Google Drive/Docs means diagrams can live directly alongside requirements documentation rather than as disconnected image exports. It is also the underlying diagram engine that AI-assisted BPMN-generation tools build on top of, so understanding the base tool helps BAs get the most out of those AI layers.

## How to use it in BA Workflows
1. **Process modeling and swimlane diagrams** - Map as-is and to-be business processes using the built-in flowchart and swimlane shape libraries, then export the diagram directly into a requirements or process document.
2. **BPMN-style workflow diagrams** - Use the flowchart/UML shape palettes to sketch workflow steps, decision points, and handoffs between roles when a full BPMN modeler (e.g. bpmn-js) is more than the stakeholder conversation needs.
3. **Stakeholder and org mapping** - Build organizational charts and RACI-style diagrams to clarify stakeholder roles and reporting lines during stakeholder analysis.
4. **Wireframing and UI mockups** - Use the mockup stencil set to sketch low-fidelity UI wireframes for requirements elicitation sessions without needing a dedicated design tool.
5. **Embedded documentation diagrams** - Embed live-editable diagrams inside Confluence pages, GitHub READMEs, or Google Docs so process diagrams stay versioned alongside the requirements they illustrate.

## Key Features
- Large built-in stencil libraries (flowcharts, UML, ER, network, mockups, org charts, Azure/AWS/GCP icons)
- Fully client-side — no account, server, or data transmission required for the browser app
- Native integrations with Confluence, Jira, GitHub, GitLab, and Google Drive/Docs/Sheets
- Desktop app, Docker image, and self-hostable .war deployment options for offline/regulated environments
- SVG-based diagrams that embed cleanly into web pages and documentation
- Free and open source under Apache-2.0 for the core editor

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** mxGraph-derived rendering engine (bundled); optional Electron shell for the desktop app
- **License:** Apache-2.0 (editor source code); bundled icon/stencil sets carry separate licensing terms

## GitHub Resources
- [jgraph/drawio](https://github.com/jgraph/drawio) - Configurable diagramming/whiteboarding client-side JavaScript editor

## Related Skills
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[ProcessPiper - Python Library for Business Process Diagrams as Code]]
