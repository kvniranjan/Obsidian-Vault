---
date: 2026-11-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-modeling, diagramming, ai-assisted-ba, workflow-automation]
source: GitHub
---

# OpenFlowKit - Local-First AI Diagramming Canvas for Process and Architecture Diagrams

## What is it?
OpenFlowKit is a free, open-source diagram canvas that lets you draw a diagram by hand, write it as code (Mermaid, D2, Structurizr), or generate it by asking any AI model, including a local one via Ollama. It is local-first with no account required, runs in the browser (app.openflowkit.com) or the terminal (`npx openflowkit`), and ships an MCP server so Claude Code and other MCP clients can edit diagrams live. It is MIT-licensed and built with React Flow and Mermaid.js.

## Why it matters for Business Analysts
BAs constantly produce flowcharts, swimlanes, and architecture-context diagrams to document current-state and future-state processes for stakeholders, and OpenFlowKit removes the friction of a paid tool or a heavyweight BPMN suite for that everyday work. Because it accepts plain-language prompts and text-based diagram code side by side with manual drawing, a BA can sketch a process quickly, hand the same diagram to a developer as Mermaid/D2 source, and export a polished PNG/SVG/PDF for a steering-committee deck. The MCP integration also means an AI assistant (e.g., Claude Code) can generate or revise process diagrams directly from a written requirement or user story, keeping diagrams in sync as requirements evolve. Its "map a GitHub repo with every arrow cited to a file and line" mode is a bonus for BAs working on technical modernization or impact-analysis efforts who need to explain existing system structure to non-technical stakeholders.

## How to use it in BA Workflows
1. **Rapid current-state/future-state flowcharting** - Sketch an as-is process flow during a stakeholder workshop, then redraw the to-be version side by side for gap analysis, without installing desktop software.
2. **AI-assisted diagram generation from requirements text** - Paste a written process description or user story into the AI prompt box and get a first-draft flowchart or sequence diagram to refine with stakeholders, cutting initial modeling time.
3. **Text-based diagrams for version control** - Author process diagrams as Mermaid or D2 code so they can live alongside requirements documents in Git and be reviewed via pull request, keeping a clean audit trail of process changes.
4. **Live diagram updates via Claude Code/MCP** - Let an AI coding assistant update a process or data-flow diagram automatically whenever related requirements or user stories change, keeping documentation current with less manual rework.
5. **Stakeholder-ready exports** - Export final diagrams as PNG, SVG, or PDF (including animated exports) for inclusion in business requirement documents, slide decks, or change-management communications.

## Key Features
- Multiple authoring modes: freehand drawing, Mermaid/D2/Structurizr code, or natural-language AI generation
- Local AI support via Ollama for offline, no-API-key diagram generation
- MCP server for live editing from Claude Desktop, Claude Code, Cursor, Windsurf, and other MCP clients
- Repo-mapping mode that ties diagram arrows to specific files and lines in a codebase
- Export to PNG, SVG, PDF, JSON, and copy-as-Mermaid
- No account or cloud dependency required; runs locally in-browser or via `npx`

## Technology Stack
- **Languages:** TypeScript, JavaScript
- **Dependencies:** React Flow, Mermaid.js, Node.js (20.11+) runtime for CLI use
- **License:** MIT

## GitHub Resources
- [openflowkit/openflowkit](https://github.com/openflowkit/openflowkit) - Free, open-source, local-first AI diagram canvas supporting Mermaid/D2/Structurizr code, AI generation, and MCP-driven live editing.

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[Drawnix - Open-Source Collaborative Whiteboard with Mind Maps and Flowcharts]]
- [[Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support]]
- [[LogicFlow - Business-Customizable Flow and Process Diagram Framework]]
