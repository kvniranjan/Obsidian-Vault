---
date: 2026-10-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, archimate, enterprise-architecture, business-architecture, modeling, togaf]
source: GitHub
---

# Archi - Open Source ArchiMate Enterprise Architecture Modelling Tool

## What is it?
Archi is a free, open-source, cross-platform tool for creating ArchiMate models — the open modeling standard hosted by The Open Group and aligned with TOGAF. Built on the Eclipse RCP platform in Java, it lets architects and analysts diagram the full ArchiMate layer stack: business, application, technology, strategy, motivation, and implementation/migration. It is one of the most widely used ArchiMate editors, with an active plugin ecosystem (including the coArchi collaboration plugin for Git-based model sharing).

## Why it matters for Business Analysts
BAs are frequently asked to connect business strategy and capability maps to the processes, applications, and data that realize them — exactly what the ArchiMate Business and Application layers are designed for. Archi gives BAs a standards-based, vendor-neutral way to model business capabilities, value streams, business processes, actors/roles, and their dependencies on application services and technology, without the licensing cost of commercial enterprise architecture suites. Because models are version-controllable XML, they fit naturally into the same Git-based workflows used by the BPMN and DMN tools already in this vault. It's a natural companion to process-modeling tools: where BPMN captures "how" a process flows, ArchiMate captures "why" it exists and "what" it depends on across the business-to-technology stack.

## How to use it in BA Workflows
1. **Business Capability Mapping** - Model the organization's business capabilities and value streams as a shared vocabulary for prioritizing initiatives and discussing scope with stakeholders.
2. **Current-State vs. Future-State Architecture** - Build "as-is" and "to-be" views of business processes, actors, and application support to communicate the impact of a proposed change.
3. **Requirements Traceability to Architecture** - Link business requirements and drivers (Motivation layer: stakeholders, drivers, goals, requirements) directly to the business processes and application services they affect, giving stakeholders a visual trace from "why" to "what."
4. **Impact Analysis** - Before approving a change request, trace an application or process element's relationships in Archi to quickly identify every upstream business process and downstream system affected.
5. **Stakeholder Communication** - Export ArchiMate viewpoints (e.g., a stakeholder view or an organization view) as lightweight diagrams for steering committee decks, avoiding the need for a full EA suite license just to produce a readable picture.

## Key Features
- Full ArchiMate 3.x notation support across all layers and relationship types
- Free-form sketch views for early-stage, informal diagramming before formal modeling
- coArchi plugin for Git-backed, multi-user collaborative model editing
- Extensible via Eclipse plugin architecture (custom properties, scripting via jArchi)
- Model Exchange File format for interoperability with other ArchiMate/TOGAF tooling
- Cross-platform desktop app (Windows, macOS, Linux)

## Technology Stack
- **Languages:** Java (Eclipse RCP/SWT)
- **Dependencies:** Eclipse Platform, Maven/Tycho build
- **License:** MIT License

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Free, open-source, cross-platform ArchiMate modelling tool with ~1.3k GitHub stars

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Stakeholder Analysis Framework]]
