---
date: 2026-10-02
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, diagrams-as-code, documentation, data-analysis]
source: GitHub
---

# Mermaid - Diagrams as Code for Flowcharts, Sequence, and Gantt Charts

## What is it?
Mermaid is a JavaScript-based diagramming and charting tool that renders diagrams from a simple, markdown-inspired text syntax. It supports more than 20 diagram types — including flowcharts, sequence diagrams, state diagrams, entity-relationship diagrams, Gantt charts, user journey maps, mindmaps, and timelines — and is natively rendered by GitHub, GitLab, Notion, and Obsidian.

## Why it matters for Business Analysts
Mermaid lets BAs produce and maintain process diagrams, decision flows, and stakeholder journey maps directly inside plain-text documents such as requirements specs, README files, or Obsidian notes — no separate modeling tool or export step required. Because diagrams are defined as version-controlled text, changes to a business process can be reviewed and diffed like any other document edit, which keeps diagrams in sync with written requirements. Its direct, built-in rendering inside Obsidian makes it especially convenient for BAs who already keep requirements and discovery notes in a vault like this one. The low barrier to entry (no drawing tools, just syntax) also makes it fast to sketch a process flow during a stakeholder interview and refine it afterward.

## How to use it in BA Workflows
1. **Process and workflow documentation** - Use `flowchart` or `graph` syntax to document "as-is" and "to-be" business processes directly in requirement documents, keeping diagrams version-controlled alongside the text they support.
2. **Stakeholder and system interaction mapping** - Use `sequenceDiagram` to show the order of interactions between stakeholders, systems, and external parties during a business process or integration.
3. **User story mapping and journey analysis** - Use `journey` diagrams to map a user's experience and satisfaction across steps of a process, useful for identifying pain points during discovery.
4. **Project and release planning** - Use `gantt` charts to communicate project timelines, milestones, and dependencies to stakeholders without needing a dedicated PM tool.
5. **Decision and state modeling** - Use `stateDiagram-v2` to model business rules and lifecycle states (e.g., an order or ticket's status transitions) that feed into decision management or DMN documentation.

## Key Features
- 20+ diagram types covering process flows, sequences, states, ER models, Gantt charts, mindmaps, and more
- Plain-text, markdown-like syntax that renders natively in GitHub, GitLab, Notion, and Obsidian
- Live editor and CLI tooling (`mermaid-live-editor`, `mermaid-cli`) for quick iteration and export to SVG/PNG
- Theming support for consistent visual style across diagrams in a document set
- Large plugin and integration ecosystem (VS Code, Confluence, Jira, documentation generators)

## Technology Stack
- **Languages:** TypeScript, JavaScript
- **Dependencies:** D3.js (rendering), Vite/ESBuild (build tooling)
- **License:** MIT

## GitHub Resources
- [mermaid-js/mermaid](https://github.com/mermaid-js/mermaid) - Core diagramming library for generating flowcharts, sequence diagrams, and more from text
- [mermaid-js/mermaid-live-editor](https://github.com/mermaid-js/mermaid-live-editor) - Browser-based live editor for previewing and sharing Mermaid diagrams
- [mermaid-js/mermaid-cli](https://github.com/mermaid-js/mermaid-cli) - Command-line tool for rendering Mermaid diagrams in automated pipelines

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[TextUSM - Text-Based Diagram Generator]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
