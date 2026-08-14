---
date: 2026-08-14
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, archimate, togaf, modeling, stakeholder-analysis]
source: GitHub
---

# Archi - Free, Open Source ArchiMate Enterprise Architecture Modelling Tool

## What is it?
Archi is a free, open source, cross-platform tool for creating models in the ArchiMate modelling language, the open enterprise architecture standard maintained by The Open Group and aligned with TOGAF. Built on the Eclipse Rich Client Platform in Java, it lets architects and analysts capture business, application, and technology layers of an organization in a single connected model, plus supporting artifacts like motivation, strategy, and implementation & migration elements.

## Why it matters for Business Analysts
Business analysts are frequently the bridge between business strategy and IT delivery, and ArchiMate gives them a standard notation to express that bridge precisely — business actors, roles, processes, and services on one side, application and technology components on the other, all explicitly linked. Archi's business layer viewpoints (actor co-operation, business process, product, and stakeholder/motivation views) let a BA model stakeholders, drivers, goals, and requirements alongside the processes and systems they affect, which is far more traceable than disconnected diagrams. Because models are stored as structured, versionable files, they integrate cleanly into a BA's existing documentation and git-based workflows. It is also a low-cost entry point for BAs working within or alongside TOGAF-based EA practices who need to produce artifacts EA teams and stakeholders will recognize.

## How to use it in BA Workflows
1. **Stakeholder and motivation modeling** - Use the Motivation layer (stakeholders, drivers, assessments, goals, outcomes, requirements, principles) to formally capture stakeholder concerns and trace them forward into business and application changes.
2. **Current-state (baseline) architecture capture** - Model existing business processes, actors, and the applications/technology that support them to produce an accurate as-is picture before proposing changes.
3. **Target-state and gap analysis** - Create target architecture views alongside the baseline and use Archi's plugins to visualize gaps, feeding directly into business case and requirements documents.
4. **Impact analysis for change requests** - Because elements are relationally connected, a BA can trace a proposed process or system change through to every dependent stakeholder, service, and application component in the model.
5. **Stakeholder communication artifacts** - Export tailored, audience-specific views (e.g., a business-process-only view for operations stakeholders vs. a full layered view for IT) as reports or images for requirements workshops and steering committees.

## Key Features
- Full ArchiMate 3.2 language support across business, application, technology, motivation, strategy, and implementation layers
- Multiple concurrent, cross-referenced viewpoints/diagrams over one underlying model, so elements stay consistent everywhere they appear
- jArchi scripting plugin for automating model generation, validation, and bulk edits via JavaScript
- coArchi plugin for git-based team collaboration and model versioning
- JasperReports-based report generation for stakeholder-ready documentation
- Cross-platform desktop app (Windows, macOS, Linux) with no server or account required

## Technology Stack
- **Languages:** Java
- **Dependencies:** Eclipse Rich Client Platform (RCP)
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - The ArchiMate Modelling Tool
- [archimatetool/archi-scripting-plugin](https://github.com/archimatetool/archi-scripting-plugin) - jArchi scripting extension
- [archimatetool/archi-modelrepository-plugin2](https://github.com/archimatetool/archi-modelrepository-plugin2) - coArchi2 collaboration plugin

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
