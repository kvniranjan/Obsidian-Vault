---
date: 2026-08-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, process-modeling, archimate, togaf, capability-mapping]
source: GitHub
---

# Archi - Open Source ArchiMate Enterprise Architecture Modelling Tool

## What is it?
Archi is a free, open-source, cross-platform tool for creating ArchiMate models — the open standard modelling language for describing enterprise architecture across business, application, and technology layers. Built on the Eclipse Rich Client Platform in Java, it is one of the most widely used ArchiMate editors and aligns with Open Group standards, including TOGAF.

## Why it matters for Business Analysts
Business analysts routinely need to place requirements and process changes in the context of the wider organization — which business capabilities, applications, and systems a change touches. Archi gives BAs a structured, standards-based way to model that context (business actors, processes, services, and their links to application and technology components) rather than relying on ad-hoc diagrams. Because it is free and MIT-licensed, it removes the licensing barrier that usually keeps EA tooling out of reach for BAs and smaller teams, letting them collaborate directly with enterprise architects using a shared notation.

## How to use it in BA Workflows
1. **Business capability mapping** - Model an organization's business capabilities and layer them against strategy or investment priorities to scope which capabilities a project or requirement set will affect.
2. **Current-state vs. future-state architecture** - Build "as-is" and "to-be" ArchiMate views to communicate the impact of a proposed change across business, application, and technology layers.
3. **Stakeholder and process impact analysis** - Trace business processes to the actors, roles, and systems that realize them, making it easier to identify who is impacted by a requirement or process redesign.
4. **Requirements traceability to architecture** - Use ArchiMate's motivation elements (drivers, goals, requirements, constraints) to link business requirements directly to the architecture elements that satisfy them.
5. **Stakeholder communication artifacts** - Generate views, reports, and diagrams from a single underlying model so different stakeholder audiences (execs, architects, delivery teams) get tailored visualizations of the same analysis.

## Key Features
- Full ArchiMate 3.x notation support across business, application, technology, and motivation layers
- Cross-platform desktop application (Windows, macOS, Linux) via Eclipse RCP
- Model repository plugin (coArchi) for Git-based collaborative modelling
- Scripting support (jArchi) for automating model creation, validation, and reporting
- CSV, SVG, and report export for sharing analysis outside the tool
- Free and open source with no licensing cost, lowering the barrier to enterprise-grade modelling

## Technology Stack
- **Languages:** Java
- **Dependencies:** Eclipse RCP, Maven (build), optional jArchi (JavaScript scripting) and coArchi (Git collaboration) plugins
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Open source ArchiMate enterprise architecture modelling tool

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[Stakeholder Analysis Framework]]
