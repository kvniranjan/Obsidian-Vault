---
date: 2026-08-06
type: skill
category: Business Analysis
tags: [business-analyst, skill, whiteboard, mind-mapping, flowchart, collaboration, process-modeling, brainstorming, requirements]
source: GitHub
---

# Drawnix — Open-Source Collaborative Whiteboard with Mind Maps and Flowcharts

## What is it?
Drawnix is an open-source, all-in-one whiteboard SaaS tool that combines mind mapping, flowcharting, and freehand drawing in a single collaborative canvas. Built with TypeScript and designed as a local-first application, it lets teams work together in real time on visual artifacts without leaving a browser tab. With over 14,000 GitHub stars, it has quickly become a go-to lightweight alternative to tools like Miro or FigJam.

## Why it matters for Business Analysts
BAs rely on visual collaboration to bridge the gap between stakeholders and technical teams — and Drawnix puts all the core modalities (mind maps, process flows, free sketches) in one place without forcing context switches between different applications. Because it is local-first, sensitive project artifacts can be captured without uploading to third-party SaaS platforms, which matters in regulated industries. The flowchart capability is directly applicable to AS-IS / TO-BE process modeling, while the mind map mode supports structured requirements brainstorming and stakeholder input capture. Its open-source nature means teams can self-host and integrate it into existing BA toolchains.

## How to use it in BA Workflows
1. **Requirements Brainstorming Sessions** - Use the mind map canvas to capture stakeholder inputs in real time during discovery workshops. Branch from a central "Problem Statement" node into themes such as Pain Points, Current Process, Desired Outcomes, and Constraints, then export the map as a structured starting point for requirements documentation.
2. **AS-IS / TO-BE Process Mapping** - Use the flowchart mode to sketch current-state business processes alongside future-state designs. The freehand annotation layer allows BAs to mark pain points, handoff gaps, or improvement opportunities directly on the diagram during walkthroughs.
3. **Impact Analysis and Dependency Mapping** - Create a whiteboard canvas per epic or initiative, mapping how a proposed change ripples across business units, systems, and stakeholder groups. Visual clusters help communicate scope and risk to non-technical sponsors.
4. **Stakeholder Workshop Facilitation** - Share a live Drawnix board with participants during remote workshops. Attendees can simultaneously add sticky-note-style freehand text, vote on ideas, and sketch alternative flows, making engagement visible in real time rather than relying on verbal input alone.
5. **Prototype Wireframe Sketching** - Use the freehand drawing tool to sketch rough UI wireframes or screen flows alongside the related requirements on the same canvas, keeping context co-located during early discovery before formal wireframes are commissioned.

## Key Features
- **All-in-one canvas** — Mind maps, flowcharts, and freehand drawing on a single infinite board
- **Local-first architecture** — Data stored locally by default; works offline and suits privacy-sensitive environments
- **Real-time collaboration** — Multi-user simultaneous editing for remote workshops and distributed teams
- **Export support** — Boards can be exported for inclusion in requirements documents and design artefacts
- **Self-hostable SaaS** — Can be deployed internally, keeping artefacts inside the organisation's boundary
- **Active development** — 14,000+ stars, 1,200+ forks, ongoing TypeScript codebase with regular releases

## Technology Stack
- **Languages:** TypeScript
- **Dependencies:** Angular/Plait board rendering engine, local-first sync
- **License:** MIT

## GitHub Resources
- [plait-board/drawnix](https://github.com/plait-board/drawnix) — All-in-one open-source whiteboard with mind maps, flowcharts, and freehand drawing

## Related Skills
- [[DDD Toolbox - EventStorming and Domain Storytelling Strategic Design Tool]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[Featmap - User Story Mapping]]
- [[TextUSM - Text-Based Diagram Generator]]
- [[ProcessPiper - Python Library for Business Process Diagrams as Code]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
