---
date: 2026-10-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, diagrams-as-code, bpmn, process-modeling, flowcharts, documentation, wireframing]
source: GitHub
---

# draw.io - Open-Source Diagramming Tool for Process and Flowchart Modeling

## What is it?
draw.io (also known as diagrams.net) is a free, open-source, client-side diagramming editor built in JavaScript. It runs entirely in the browser or as a desktop app with no server dependency, and natively supports flowcharts, BPMN, UML, ER diagrams, network diagrams, and wireframes, saving files as portable `.drawio`, `.xml`, `.svg`, or `.png`.

## Why it matters for Business Analysts
draw.io is one of the most widely adopted diagramming tools in enterprise BA work because it requires no license cost, no account, and integrates directly into tools BAs already use — Confluence, SharePoint, Google Drive, and GitHub. Its BPMN shape library and built-in flowchart stencils let BAs produce as-is/to-be process maps, swimlane diagrams, and wireframes quickly without learning a dedicated modeling suite. Because diagrams are stored as readable XML/SVG, they can be version-controlled, diffed, and embedded directly into requirements documents, making them easy to maintain across iterative stakeholder reviews.

## How to use it in BA Workflows
1. **As-Is / To-Be Process Mapping** - Use the BPMN and flowchart shape libraries to document current-state and future-state business processes side-by-side for gap analysis presentations.
2. **Swimlane and Cross-Functional Diagrams** - Build swimlane diagrams that assign process steps to roles or departments, clarifying handoffs and responsibilities (RACI-style) during process workshops.
3. **Wireframing and UI Mockups** - Use the built-in mockup/wireframe shape set to sketch screen layouts quickly when gathering UI requirements with stakeholders, without needing a separate design tool.
4. **Data and System Diagrams** - Create ER diagrams and system context diagrams to document data models and integration points as part of functional specifications.
5. **Embedded Living Documentation** - Embed draw.io diagrams directly into Confluence pages, GitHub Markdown, or Google Docs so that process visuals stay attached to the requirements they support and can be edited in place by any stakeholder.

## Key Features
- **Zero-cost, no account required** — fully free and open source, usable offline via desktop app or self-hosted
- **BPMN, UML, ER, flowchart, and wireframe shape libraries** — covers most BA diagramming needs in one tool
- **Readable file format** — diagrams stored as XML/SVG, enabling version control and diffing in Git repositories
- **Deep integrations** — native plugins for Confluence, Jira, SharePoint, Google Drive, GitHub, and VS Code
- **Real-time collaboration** — multiple stakeholders can co-edit diagrams simultaneously in supported integrations
- **Export flexibility** — export to PNG, SVG, PDF, or editable XML for inclusion in any BA deliverable

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** mxGraph (underlying graph visualization library); Electron for desktop builds
- **License:** Apache 2.0

## GitHub Resources
- [jgraph/drawio](https://github.com/jgraph/drawio) - Core open-source draw.io/diagrams.net diagramming editor

## Related Skills
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[bpmn-io Web Modeler]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
