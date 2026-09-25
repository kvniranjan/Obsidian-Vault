---
date: 2026-09-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, archimate, process-modeling, togaf]
source: GitHub
---

# Archi - Open-Source ArchiMate Enterprise Architecture Modeling Tool

## What is it?
Archi is a free, open source, cross-platform desktop tool for creating models in the ArchiMate enterprise architecture modeling language, an open standard maintained by The Open Group. It has been under active development since 2010 and is widely regarded as the reference free tool for ArchiMate, used by architects and analysts working within TOGAF and other EA frameworks.

## Why it matters for Business Analysts
Business Analysts are frequently asked to document how business processes, capabilities, applications, and data connect to strategic goals — exactly what ArchiMate's business, application, and technology layers are designed to capture. Archi lets a BA build formal, standards-based views (capability maps, business process diagrams, stakeholder/motivation viewpoints) that plug directly into enterprise architecture and requirements traceability work, rather than relying on free-form diagrams that architects have to reinterpret. Its motivation and strategy layers explicitly model stakeholders, drivers, goals, and requirements — bridging BA deliverables with formal architecture artifacts. Because it's free and cross-platform, teams can standardize on it without licensing costs typically associated with commercial EA suites.

## How to use it in BA Workflows
1. **Capability and Value Stream Mapping** - Model business capabilities and value streams to support strategic planning, gap analysis, and roadmap discussions with stakeholders.
2. **Business Process Documentation** - Use the Business Layer to diagram business processes, functions, and actors, linking them to the applications and services that support them.
3. **Requirements and Motivation Modeling** - Use the Motivation extension to capture stakeholders, drivers, goals, outcomes, and requirements as first-class model elements traceable to the architecture they justify.
4. **Impact and Traceability Analysis** - Leverage Archi's model relationships and analysis views to trace how a proposed change to a process or application ripples through to other elements, supporting change-impact assessments.
5. **Stakeholder Viewpoints** - Generate tailored viewpoints (e.g., a business-only view or an application landscape view) from the same underlying model to communicate with different audiences without maintaining separate diagrams.

## Key Features
- Full support for the ArchiMate 3.x specification across business, application, technology, motivation, strategy, and implementation layers
- Free-form drawing (Sketch views) alongside formal ArchiMate diagrams for early-stage brainstorming
- Model validation and relationship consistency checking
- Export to CSV, SVG, and formatted HTML/PDF reports for stakeholder distribution
- jArchi scripting plugin for automating model generation and bulk edits
- coArchi plugin for Git-based collaborative model versioning and team editing

## Technology Stack
- **Languages:** Java (Eclipse RCP platform)
- **Dependencies:** Eclipse SWT/RCP framework; optional jArchi (JavaScript/Nashorn) and coArchi (Git) plugins
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - The core Archi ArchiMate modelling tool
- [archimatetool/archi-scripting-plugin](https://github.com/archimatetool/archi-scripting-plugin) - jArchi scripting plugin for automation
- [archimatetool/archi-modelrepository-plugin2](https://github.com/archimatetool/archi-modelrepository-plugin2) - coArchi2 plugin for Git-based collaboration on models

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Stakeholder Analysis Framework]]
