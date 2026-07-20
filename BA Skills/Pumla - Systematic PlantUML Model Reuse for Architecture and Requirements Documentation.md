---
date: 2026-07-20
type: skill
category: Business Analysis
tags: [business-analyst, skill, plantuml, architecture-modeling, requirements-tracing, documentation, c4-model, diagrams-as-code]
source: GitHub
---

# Pumla - Systematic PlantUML Model Reuse for Architecture and Requirements Documentation

## What is it?
Pumla is an open-source Python tool that enables systematic re-use of PlantUML model elements across an entire project or documentation set. It scans a directory tree for PlantUML definitions, indexes them as JSON, and lets you include any element in any diagram without duplication. This brings a "single source of truth" discipline to architecture and requirements diagrams.

## Why it matters for Business Analysts
BAs frequently maintain multiple overlapping diagrams — context diagrams, process flows, data models, stakeholder maps — that share the same components (systems, actors, databases, processes). Pumla eliminates the need to re-draw or re-define these elements in each diagram, keeping all views consistent when a system or process name changes. It natively supports the C4 model for architecture documentation, which BAs use to communicate system context to both technical and business audiences. Its traceability features also allow linking requirements to model elements, bridging the gap between requirements documentation and architectural design.

## How to use it in BA Workflows
1. **Single-Source Architecture Catalog** - Define each system, actor, and component once in a dedicated `.puml` file; pumla auto-discovers and catalogs them so every context, container, or component diagram references the same definition.
2. **Cross-Diagram Consistency Enforcement** - When a stakeholder or system name changes, update only the source definition; all diagrams that include it regenerate correctly without manual find-and-replace across files.
3. **Requirements-to-Model Traceability** - Tag model elements with requirement IDs or metadata; pumla's JSON index can be queried to produce traceability matrices showing which architectural elements satisfy which requirements.
4. **C4 Model Documentation** - Use built-in C4 support to produce Context, Container, and Component diagrams at multiple levels of detail — ideal for BA deliverables targeted at executive, business, and technical audiences simultaneously.
5. **Architecture Decision Records (ADR) Integration** - Link pumla model elements to ADR files so stakeholders can trace why a particular design choice was made, providing rich context for change-impact analysis.

## Key Features
- **Auto-Discovery** — recursively scans directory trees and indexes all PlantUML element definitions automatically
- **JSON Metadata Index** — exports a structured JSON catalog of all model elements, enabling scripting, reporting, and traceability queries
- **C4 Model Support** — first-class support for C4 Context, Container, and Component diagram types
- **Re-usable Element Includes** — include any cataloged element into any diagram with a single macro, no copy-paste
- **Markdown Integration** — model elements and descriptions can be embedded in Markdown documentation alongside diagrams
- **Filtering and Tagging** — tag elements by type, layer, or domain; filter diagrams to show only relevant subsets
- **PlantUML Native** — no new diagramming syntax; works entirely within PlantUML's ecosystem

## Technology Stack
- **Languages:** Python, PlantUML
- **Dependencies:** Python 3, PlantUML (local or server), Jinja2 for templating
- **License:** MIT

## GitHub Resources
- [DrMarkusVoss/pumla](https://github.com/DrMarkusVoss/pumla) - Systematic re-use of PlantUML model elements across architecture and documentation projects

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[TRLC - Treat Requirements Like Code with a Domain-Specific Language]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
