---
date: 2026-03-23
type: skill
category: Business Analysis
tags: [business-analyst, skill, user-story-mapping, diagramming, requirements, agile]
source: GitHub
---

# TextUSM - Text-Based Diagram Generator

## What is it?
TextUSM is an open-source online tool that generates professional BA diagrams from simple indented text. Type structured plain text, and it renders diagrams instantly — no drag-and-drop, no mouse-heavy UI. Available as a web app, browser extension, and CLI tool.

GitHub: [harehare/textusm](https://github.com/harehare/textusm)

## Why it matters for Business Analysts
BAs often need to produce multiple diagram types rapidly during workshops, sprint planning, and stakeholder meetings. TextUSM lets you stay keyboard-focused and generate any of 15+ diagram types without context-switching to a separate design tool. Its text-first approach also makes diagrams version-controllable (store `.usm` files in git alongside requirements docs).

## How to use it in BA Workflows

### Quick Start (Web)
1. Go to the hosted app or self-host via Docker
2. Select diagram type from the sidebar
3. Type indented text — each indentation level maps to a hierarchy level

### User Story Map Example
```
User Activities
  User Tasks
    User Story 1
    User Story 2
  Another Task
    User Story 3
```

### Business Model Canvas Example
```
Key Partners
  Partner A
Key Activities
  Activity 1
Value Propositions
  Value 1
```

### CLI Usage (for automation pipelines)
```bash
textusm --type usm --input stories.txt --output diagram.svg
```

### Workshop Facilitation Tip
Share your screen while typing — stakeholders see the diagram build in real time, making elicitation sessions more collaborative and visual.

## Key Features
- **15+ diagram types** including User Story Map, Business Model Canvas, Opportunity Canvas, Empathy Map, Mind Map, Impact Map, Gantt Chart, ER Diagram, Kanban, Sequence Diagram, and more
- **Export as PNG or SVG** for use in documents, presentations, and Confluence pages
- **Keyboard-driven** — Tab to indent, Shift+Tab to unindent; no mouse required
- **CLI support** for batch diagram generation and CI/CD integration
- **Self-hostable** via Docker for organizations with data residency requirements
- **Browser extension** for quick access without navigating to the web app
- **Open source** (MIT license) — customizable and free

## Diagram Types Relevant to BAs

| Diagram | BA Use Case |
|---|---|
| User Story Map | Sprint planning, backlog structuring |
| Business Model Canvas | As-Is / To-Be analysis |
| Opportunity Canvas | Problem/solution framing for new features |
| Empathy Map | Stakeholder/user research synthesis |
| Impact Map | Goal → actor → impact → deliverable tracing |
| Gantt Chart | Project timeline visualization |
| Kanban | Work-in-progress tracking |
| Mind Map | Requirements brainstorming |
| ER Diagram | Data model documentation |

## GitHub Resources
- [harehare/textusm](https://github.com/harehare/textusm) — Main repository with web app, CLI, and browser extension

## Related Skills
- [[Featmap - User Story Mapping]]
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
