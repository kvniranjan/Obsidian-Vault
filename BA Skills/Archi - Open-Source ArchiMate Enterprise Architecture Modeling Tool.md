---
date: 2026-11-20
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, archimate, modeling, process-modeling]
source: GitHub
---

# Archi - Free ArchiMate Enterprise Architecture Modelling Tool

## What is it?
Archi is a free, open-source, cross-platform tool for creating ArchiMate models, the open standard notation for enterprise architecture maintained by The Open Group. Built on the Eclipse platform in Java, it lets analysts model business, application, and technology layers in a single, consistent notation, and has been a reference implementation for the ArchiMate Model Exchange File Format.

## Why it matters for Business Analysts
BAs are regularly asked to connect business requirements to the systems, processes, and capabilities that deliver them, and ArchiMate gives a standardized visual language for exactly that layered view (business/application/technology). Archi makes this accessible without a costly EA suite license, so a BA can map current-state and target-state architectures, business capabilities, and process-to-system dependencies directly. Its model repository plugin (Git-backed, XML-based "Grafico" format) also lets architecture models be version-controlled and diffed like code, which fits well alongside requirements and process artifacts already tracked in a repo.

## How to use it in BA Workflows
1. **Capability and value-stream mapping** - Model business capabilities, value streams, and how they're realized by applications and infrastructure to support capability-gap analysis in business cases.
2. **Current-state vs. target-state architecture** - Build "as-is" and "to-be" ArchiMate views side by side to communicate the impact of a proposed initiative to stakeholders and architects.
3. **Requirements-to-architecture traceability** - Link business requirements and drivers to the specific application components or business processes that satisfy them, using ArchiMate's motivation layer (drivers, goals, requirements, constraints).
4. **Stakeholder and impact analysis** - Use ArchiMate's stakeholder and assessment elements to document who is affected by a change and visualize downstream impact across business and technology layers.
5. **Process-to-system handoff diagrams** - Model how BPMN-level business processes map onto application services and technology components, bridging process modeling tools (e.g. bpmn-js, Camunda Modeler) with the broader architecture view.

## Key Features
- Full ArchiMate 3.x notation support across business, application, technology, motivation, and strategy layers
- Free, cross-platform desktop application (Windows, macOS, Linux) with no licensing cost
- Model views, diagrams, and reports generated directly from the underlying model (single source of truth)
- Plugin ecosystem, including a Git-based model repository plugin for version-controlled, collaborative architecture modeling
- Supports the Open Group's ArchiMate Model Exchange File Format for interoperability with other EA tools
- Active governance and community maintenance under the Archi project

## Technology Stack
- **Languages:** Java (Eclipse RCP platform)
- **Dependencies:** Eclipse Platform, Java SE runtime
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Core Archi editor for creating ArchiMate enterprise architecture models
- [archimatetool/archi-modelrepository-plugin](https://github.com/archi-contribs/archi-modelrepository-plugin) - Git-based collaborative model repository plugin for Archi

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Stakeholder Analysis Framework]]
