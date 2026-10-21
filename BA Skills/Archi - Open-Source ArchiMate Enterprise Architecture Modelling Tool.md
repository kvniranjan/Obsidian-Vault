---
date: 2026-10-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, archimate, enterprise-architecture, process-modeling, stakeholder-analysis, modeling, java]
source: GitHub
---

# Archi - Open-Source ArchiMate Enterprise Architecture Modelling Tool

## What is it?
Archi is a free, open-source editor for creating ArchiMate models and diagrams, built on the Eclipse RCP platform. It implements the full ArchiMate 3.x specification — spanning the Business, Application, Technology, Motivation, and Strategy layers — and has been a mainstay of the enterprise architecture community for over a decade. It runs cross-platform on Windows, macOS, and Linux as a standalone desktop application.

## Why it matters for Business Analysts
ArchiMate's Business Layer is purpose-built for the kind of modeling BAs do daily: business processes, actors, roles, services, and the stakeholder/motivation elements (drivers, goals, requirements, constraints) that justify why a change is needed. Archi lets a BA model current-state ("as-is") and future-state ("to-be") business architecture side by side with the application and technology layers that implement it, making impact analysis and gap analysis concrete rather than narrative. Its model repository plugin (coArchi) supports Git-based collaborative modeling, so BA deliverables can be version-controlled and reviewed like code. Being free and MIT-licensed removes the cost barrier that typically gates enterprise architecture tooling (e.g., Sparx EA, BiZZdesign) away from BA teams.

## How to use it in BA Workflows
1. **Business Process and Capability Mapping** - Model business processes, functions, and capabilities in the Business Layer, and link them to the application services and components that realize them, giving a clear capability-to-system traceability view.
2. **Stakeholder and Motivation Modeling** - Use Motivation Layer elements (stakeholder, driver, assessment, goal, requirement, constraint) to formally capture why a project exists and tie it directly to the business and solution elements it drives.
3. **As-Is / To-Be Architecture Comparison** - Maintain parallel baseline and target-state views to communicate transformation scope, gaps, and migration roadmaps to sponsors and steering committees.
4. **Impact and Gap Analysis** - Leverage ArchiMate's cross-layer relationships to trace how a proposed change in a business process cascades into application and technology dependencies before committing to a solution design.
5. **Collaborative Architecture Repositories** - Use the coArchi plugin to store ArchiMate models in Git repositories, enabling version history, branching, and peer review of architecture artifacts alongside other project documentation.

## Key Features
- Full ArchiMate 3.x specification support across Business, Application, Technology, Motivation, and Strategy layers
- Model views, viewpoints, and diagram generation for stakeholder-specific communication
- coArchi plugin for Git-based collaborative model versioning
- jArchi scripting plugin for automating model validation, bulk edits, and report generation
- Model Exchange Format (Open Group standard) import/export for interoperability with other EA tools
- Extensible plugin architecture via Eclipse RCP
- Cross-platform desktop application (Windows, macOS, Linux)

## Technology Stack
- **Languages:** Java
- **Dependencies:** Eclipse RCP/SWT, Maven/Tycho build
- **License:** MIT License

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Archi: free, open-source ArchiMate enterprise architecture modelling tool (~1.3k stars)

## Related Skills
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Stakeholder Analysis Framework]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
