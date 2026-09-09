---
date: 2026-09-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, bpmn, diagramming, whiteboarding]
source: GitHub
---

# draw.io - Open-Source Diagramming and Whiteboarding Platform

## What is it?
draw.io (also known as diagrams.net) is a free, open-source, client-side diagramming and whiteboarding application that runs entirely in the browser with no server-side processing of diagram data. It ships as a web app, an Electron desktop app, a Confluence/Jira plugin, and embeddable widgets, and stores diagrams as portable XML that can be embedded directly in PNG or SVG files.

## Why it matters for Business Analysts
draw.io is one of the most widely used free tools for producing process flows, BPMN diagrams, org charts, wireframes, ER diagrams, and swimlane diagrams — the everyday visual artifacts a BA produces for requirements documents and stakeholder workshops. Because files can be saved to Google Drive, OneDrive, GitHub, GitLab, or plain local disk, BAs can version-control their diagrams alongside requirements text rather than relying on a proprietary hosted tool. Its shape libraries (including a native BPMN stencil set) and the ability to import Visio files lower the barrier for teams migrating off commercial modeling software, and its Confluence/Jira integration lets diagrams live directly next to requirements and user stories.

## How to use it in BA Workflows
1. **Process and BPMN modeling** - Use the built-in BPMN shape library to model as-is and to-be business processes, decision points, and swimlanes for process improvement work.
2. **Requirements and architecture diagrams** - Produce context diagrams, data flow diagrams, ER diagrams, and system architecture sketches to accompany a BRD or FRD.
3. **Stakeholder workshops and whiteboarding** - Use the whiteboard/freehand mode during discovery sessions to capture stakeholder input live, then formalize it into a structured diagram afterward.
4. **Docs-as-code diagram versioning** - Store the underlying `.drawio` XML in git alongside markdown requirements so diagram history is reviewable and diffable, mirroring the docs-as-code pattern used by tools like Sphinx-Needs.
5. **Embedding in wikis and tickets** - Use the Confluence and Jira plugins (or the GitHub/GitLab integration) to keep diagrams synchronized with the requirements and stories they illustrate, avoiding stale screenshots.

## Key Features
- Native BPMN, UML, ER, and flowchart shape libraries out of the box
- Fully client-side — no diagram data sent to a server, useful for confidential BA artifacts
- Diagrams stored as portable XML embedded in PNG/SVG, so a single exported image is also the editable source file
- Multiple storage backends: Google Drive, OneDrive, GitHub, GitLab, Dropbox, or local disk
- Desktop (Electron), web, and Confluence/Jira plugin distributions
- Visio (.vsdx) import/export for teams migrating from commercial tools

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** Apache 2.0-compatible third-party JS libraries (no GPL/AGPL dependencies)
- **License:** Apache License 2.0 (icon/stencil sets carry additional usage restrictions for Atlassian marketplace products)

## GitHub Resources
- [jgraph/drawio](https://github.com/jgraph/drawio) - The core draw.io/diagrams.net client-side diagram editor

## Related Skills
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[BPMN Process Designer - Vue.js Extended BPMN Modeler Built on bpmn-js]]
