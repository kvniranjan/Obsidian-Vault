---
date: 2026-08-23
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, bpmn, diagramming, visualization]
source: GitHub
---

# draw.io - Open-Source Diagramming Editor for Process and Requirements Visualization

## What is it?
draw.io (also known as diagrams.net) is a free, open-source, client-side diagramming editor built in JavaScript that runs entirely in the browser with no account or server dependency required. It ships with a library of roughly 10,000 shapes spanning BPMN, UML, ER diagrams, flowcharts, network topology, and cloud architecture (AWS, Azure, GCP), and can save diagrams to local disk, Git repositories, Confluence, Google Drive, or OneDrive.

## Why it matters for Business Analysts
draw.io is one of the most widely adopted free diagramming tools in the world, making it a low-friction default for BAs who need to produce process maps, swimlane diagrams, and stakeholder or system context diagrams without procuring commercial licenses like Visio or Lucidchart. Its BPMN shape set lets BAs sketch "as-is" and "to-be" process flows using standard notation that developers and process owners both recognize. Because diagrams are stored as portable XML files, they integrate cleanly into version-controlled documentation and wikis (Confluence, GitHub) rather than living in siloed desktop files. The offline, client-side architecture also makes it a safe choice in regulated or security-conscious enterprises where diagram content cannot leave the local machine.

## How to use it in BA Workflows
1. **Process Modeling** - Use the BPMN shape library to draft as-is and to-be business process diagrams with correct pools, lanes, gateways, and events for stakeholder review.
2. **Requirements Visualization** - Create system context diagrams, data flow diagrams, and entity-relationship diagrams to accompany written requirements and reduce ambiguity.
3. **Stakeholder Communication** - Build simple flowcharts and org charts to walk non-technical stakeholders through a workflow during requirements workshops.
4. **Living Documentation** - Embed draw.io diagrams directly in Confluence pages or Git-backed repos (via .drawio XML files) so process diagrams stay versioned alongside requirements documents.
5. **Rapid Prototyping** - Sketch wireframes and UI mockups quickly during discovery sessions before handing designs off to UX or development teams.

## Key Features
- ~10,000 built-in shapes covering BPMN, UML, ER, network, cloud architecture, and P&ID notations
- Fully client-side editor - no account, server, or internet connection required to use
- Direct save/sync integrations with GitHub, GitLab, Confluence, Google Drive, and OneDrive
- Diagrams stored as portable, human-readable XML for easy version control and diffing
- Available as a web app, Electron desktop app (drawio-desktop), and embeddable component
- Export to PNG, SVG, PDF, and other common formats for sharing in documents and presentations

## Technology Stack
- **Languages:** JavaScript (client-side editor), built on the mxGraph library
- **Dependencies:** Electron (desktop build), various minified JS libraries
- **License:** Apache 2.0 (with CC BY 4.0 for JGraph-provided icons/templates)

## GitHub Resources
- [jgraph/drawio](https://github.com/jgraph/drawio) - The core client-side draw.io/diagrams.net editor

## Related Skills
- [[BPMN Process Designer - Vue.js Extended BPMN Modeler Built on bpmn-js]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
