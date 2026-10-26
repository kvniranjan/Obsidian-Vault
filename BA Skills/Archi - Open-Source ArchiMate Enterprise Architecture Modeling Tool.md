---
date: 2026-10-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, archimate, enterprise-architecture, togaf, stakeholder-analysis, process-modeling, modeling]
source: GitHub
---

# Archi - Open-Source ArchiMate Enterprise Architecture Modeling Tool

## What is it?
Archi is a free, open-source, cross-platform modeling tool for creating ArchiMate models and diagrams. ArchiMate is an open enterprise architecture modeling standard hosted by The Open Group and aligned with frameworks like TOGAF, and Archi is the most widely adopted free implementation of it. It is built on the Eclipse platform and runs on Windows, macOS, and Linux.

## Why it matters for Business Analysts
ArchiMate's layered viewpoints map directly onto core BA deliverables: the Business layer models business processes, functions, and services; the Motivation layer formally captures stakeholders, drivers, goals, requirements, and constraints; and the Application/Technology layers trace how those business needs are realized by systems. This gives BAs a single, standards-based tool to connect "why" (stakeholder motivation), "what" (business process and capability), and "how" (application and technology landscape) rather than juggling separate BPMN and requirements tools. Because Archi is free and vendor-neutral, it lowers the barrier to enterprise-grade architecture work compared to commercial tools like Enterprise Architect or Visio, and its coArchi plugin enables Git-based collaborative modeling across distributed BA and architecture teams.

## How to use it in BA Workflows
1. **Stakeholder and Motivation Modeling** - Use the Motivation layer to formally model stakeholders, their concerns, drivers, assessments, goals, outcomes, requirements, and constraints, producing a traceable rationale for why a change initiative exists.
2. **Business Process and Capability Mapping** - Model business processes, functions, services, and actors in the Business layer to document current-state and future-state operating models alongside capability maps.
3. **Requirements-to-Solution Traceability** - Link Motivation-layer requirements to Business-layer processes and Application-layer components, giving stakeholders an end-to-end view from business need to implemented solution.
4. **Gap Analysis and Roadmapping** - Use the Implementation & Migration layer (plateaus, gaps, work packages) to compare baseline and target architectures and communicate transformation roadmaps to sponsors.
5. **Collaborative Architecture Repositories** - Pair Archi with the coArchi plugin to version-control shared ArchiMate models in Git, enabling distributed BA/EA teams to collaborate on the same model without conflicts.

## Key Features
- Full ArchiMate 3.x specification support across Strategy, Business, Application, Technology, Physical, Motivation, and Implementation & Migration layers
- Model views/viewpoints for tailoring diagrams to specific stakeholder audiences
- Model Relations and Analysis views for impact and dependency analysis
- jArchi scripting engine for automating model validation, bulk edits, and report generation
- coArchi plugin for Git-based collaborative model repositories
- Export to image formats, CSV, and model exchange formats for interoperability
- Free and open source under the MIT license, with an active plugin ecosystem

## Technology Stack
- **Languages:** Java (built on the Eclipse RCP platform)
- **Dependencies:** Eclipse Platform; optional plugins — coArchi (Git collaboration), jArchi (JavaScript scripting)
- **License:** MIT License

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Free, open-source ArchiMate enterprise architecture modeling tool (1.3k stars)

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[Stakeholder Analysis Framework]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
