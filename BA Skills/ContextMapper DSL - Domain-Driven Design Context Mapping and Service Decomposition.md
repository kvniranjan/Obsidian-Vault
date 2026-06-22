---
date: 2026-06-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, domain-driven-design, context-mapping, service-decomposition, dsl, modeling, architecture]
source: GitHub
---

# ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition

## What is it?
ContextMapper is an open-source project providing a Domain-Specific Language (DSL) and tooling built on Domain-Driven Design (DDD) patterns for context mapping and service decomposition. It lets architects and analysts describe bounded contexts, their relationships, and integration patterns in a structured, code-like format called CML (Context Mapper Language). The tool generates UML diagrams, service contracts, and even microservice decomposition proposals from a single source-of-truth model.

## Why it matters for Business Analysts
Business Analysts working on complex enterprise systems or digital transformation initiatives often struggle to document domain boundaries and system integration points in a way that stays in sync with development. ContextMapper bridges that gap by giving BAs a structured, version-controllable way to capture bounded contexts, domain ownership, and upstream/downstream relationships — the core artifacts of strategic DDD. Because models are text-based, they live in Git alongside code, preventing the typical drift between BA documentation and the actual system. The built-in generators produce stakeholder-ready UML context maps automatically, eliminating manual diagram maintenance.

## How to use it in BA Workflows
1. **Domain Boundary Mapping** - Write CML files to define each Bounded Context (e.g., `OrderManagement`, `CustomerProfile`) and their team ownership. Use relationship patterns like Partnership, Customer-Supplier, or Anti-Corruption Layer to document how systems integrate, producing a living architecture diagram all stakeholders can reference.
2. **As-Is / To-Be Architecture Documentation** - Model the current system landscape in CML as a baseline, then create a separate To-Be model capturing desired domain decomposition. Diff the two models in Git to communicate change impact to stakeholders clearly and traceably.
3. **Microservice Decomposition Analysis** - Use the built-in Service Cutter integration to input your bounded context model and receive data-driven proposals for how to split a monolith into services, giving BAs objective input for architectural roadmap discussions.
4. **Generating UML and PlantUML Diagrams** - Run the generators to auto-produce context map diagrams, class diagrams for aggregates, and PlantUML files. Embed these in requirements documents or Confluence pages, knowing they are always regenerated from the authoritative CML model rather than manually drawn.
5. **Ubiquitous Language Enforcement** - Use the CML Aggregate and Entity definitions to codify the ubiquitous language agreed between business and development. When domain terms change, updating the CML model propagates those changes to generated contracts and diagrams, keeping documentation and glossaries consistent.

## Key Features
- **CML Language** - Human-readable DSL for defining Bounded Contexts, Aggregates, Entities, and inter-context relationships using strategic DDD patterns
- **Context Map Generators** - Auto-generates PlantUML and Graphviz context map diagrams from CML models
- **Service Cutter Integration** - Provides algorithmic microservice decomposition recommendations based on coupling criteria in the model
- **MDSL Service Contract Generation** - Generates Microservice Domain-Specific Language (MDSL) API contracts from bounded context definitions
- **VS Code & Eclipse Support** - Available as IDE extensions with syntax highlighting, validation, and diagram preview
- **Architectural Refactoring** - Built-in model refactorings (e.g., split bounded context, merge contexts) to evolve the model as understanding improves
- **Event Storming Integration** - CML supports importing Event Storming output directly to bootstrap a context map from collaborative modeling sessions

## Technology Stack
- **Languages:** Java (core DSL engine, Xtext-based), CML (the modeled language itself)
- **Dependencies:** Eclipse Xtext framework, Graphviz (for diagram rendering), PlantUML
- **License:** Apache License 2.0

## GitHub Resources
- [ContextMapper/context-mapper-dsl](https://github.com/ContextMapper/context-mapper-dsl) - Core DSL engine, VS Code and Eclipse plugin, and diagram generators (261 stars)

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[TextUSM - Text-Based Diagram Generator]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[Camunda - BPMN Process Orchestration Framework]]
