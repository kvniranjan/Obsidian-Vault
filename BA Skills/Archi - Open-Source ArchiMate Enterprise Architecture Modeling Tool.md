---
date: 2026-10-20
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, archimate, togaf, process-modeling, stakeholder-analysis]
source: GitHub
---

# Archi - Free ArchiMate Enterprise Architecture Modeling Tool

## What is it?
Archi is a free, open-source, cross-platform editor for building models in the ArchiMate® modeling language, the Open Group standard for describing enterprise architecture. It lets architects and analysts capture business, application, and technology layers of an organization in a single, interconnected model, and is commonly used alongside or within a TOGAF® enterprise architecture framework.

## Why it matters for Business Analysts
Business Analysts are often asked to bridge business strategy and IT delivery, and ArchiMate gives them a standard vocabulary for doing that — business actors, roles, processes, services, and data objects connected to the applications and infrastructure that realize them. Archi makes it possible to visually trace how a stakeholder's goal connects to a business capability, down to the systems and processes that deliver it, which is invaluable for impact analysis, capability mapping, and current-state/future-state (as-is/to-be) comparisons. Because it is free and standards-based, BAs can produce architecture artifacts that are portable and reviewable by enterprise architects without needing a commercial license.

## How to use it in BA Workflows
1. **Capability and value-stream mapping** - Model business capabilities, value streams, and the services/processes that support them to show stakeholders how strategic goals cascade into operational delivery.
2. **Stakeholder and motivation modeling** - Use ArchiMate's Motivation layer (stakeholders, drivers, goals, requirements, principles) to document who cares about a change and why, directly linking requirements to the business drivers that justify them.
3. **As-is / to-be architecture comparison** - Build separate current-state and target-state views to visualize the gap analysis behind a transformation initiative, supporting business case and roadmap discussions.
4. **Application and data impact analysis** - Trace a proposed process or requirement change through application components and data objects to identify downstream systems affected, feeding into scope and risk assessments.
5. **Requirements traceability views** - Link requirements elements to the business processes, application services, and technology nodes that realize them, giving a visual, reviewable traceability matrix alongside a traditional requirements register.

## Key Features
- Full ArchiMate 3.x notation support across Business, Application, Technology, Motivation, Strategy, and Implementation & Migration layers
- Multiple concurrent views/diagrams over one underlying model, so a single element (e.g., a business process) stays consistent across every diagram that references it
- Model collaboration via the Archi coArchi plugin for Git-based sharing and versioning of models among a team
- Report generation (HTML/CSV) for publishing architecture documentation to stakeholders without requiring them to open the tool
- Extensible via a plugin architecture (jArchi scripting support for automation and bulk model edits)
- Cross-platform desktop application (Windows, macOS, Linux) built on the Eclipse RCP framework

## Technology Stack
- **Languages:** Java (Eclipse RCP/SWT)
- **Dependencies:** Eclipse Platform, optional coArchi/jArchi plugins for Git collaboration and JavaScript scripting
- **License:** MIT License

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Free, open-source ArchiMate enterprise architecture modeling tool aligned with TOGAF

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Stakeholder Analysis Framework]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
