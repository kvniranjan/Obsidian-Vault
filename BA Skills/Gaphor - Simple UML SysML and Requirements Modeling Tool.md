---
date: 2026-07-19
type: skill
category: Business Analysis
tags: [business-analyst, skill, uml, sysml, requirements, modeling, diagramming, python, c4-model]
source: GitHub
---

# Gaphor - Simple UML, SysML, and Requirements Modeling Tool

## What is it?
Gaphor is a free, open-source modeling application written in Python that supports UML 2, SysML, C4 architecture diagrams, and RAAML standards. It provides a graphical environment for creating fully-compliant UML 2 data models, going well beyond simple picture drawing to enforce model semantics. Available on Windows, macOS, and Linux, Gaphor is designed to be approachable for beginners while remaining powerful enough for professional modeling work.

## Why it matters for Business Analysts
BAs frequently need to document system behavior, data structures, stakeholder interactions, and requirements in a standards-based format that developers and architects can act on. Gaphor's requirements diagrams (via SysML) let analysts formally capture and link requirements to system components in the same tool used for system architecture. Its support for UML use case, sequence, and class diagrams covers the most common BA deliverables without requiring expensive tools like Enterprise Architect or Visio. Being Apache 2 licensed and Python-based means BAs can automate diagram generation from scripts or integrate Gaphor models into Jupyter notebook workflows for requirements traceability analysis.

## How to use it in BA Workflows
1. **Requirements Diagrams (SysML)** - Use SysML block definition and requirements diagrams to formally document functional and non-functional requirements, trace them to system components, and generate traceability matrices for stakeholder sign-off.
2. **Use Case and Actor Modeling** - Draw UML use case diagrams to visually map system actors, user interactions, and system scope boundaries — ideal for scope definition workshops and sign-off sessions with business stakeholders.
3. **Process Sequence Diagrams** - Create interaction/sequence diagrams to document end-to-end business process flows, API handoffs, and system integration points that complement BPMN process models.
4. **Data and Domain Modeling** - Build UML class diagrams to capture business domain entities, attributes, relationships, and multiplicity — feeding downstream data dictionary and ERD documentation for solution design.
5. **Architecture Context (C4 Model)** - Produce C4 context and container diagrams to communicate system landscape and integration architecture to business and technical stakeholders at the right level of abstraction.

## Key Features
- Full UML 2 compliance — enforces model semantics, not just drawing shapes
- SysML requirements diagrams for formal requirements traceability
- C4 model support for lightweight architecture communication
- RAAML support for safety and risk analysis modeling
- Export to PDF, PNG, SVG, and XML formats
- Python scripting API and Jupyter notebook integration for automated model processing
- Plugin architecture for extending diagram types and exporters
- Cross-platform: Windows, macOS, and Linux

## Technology Stack
- **Languages:** Python
- **Dependencies:** GTK4, Cairo (rendering), Python packaging via pip
- **License:** Apache License 2.0

## GitHub Resources
- [gaphor/gaphor](https://github.com/gaphor/gaphor) - The simple modeling tool: UML, SysML, C4, and requirements diagrams in one open-source Python application (2.2k stars)

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
