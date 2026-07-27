---
date: 2026-07-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, domain-driven-design, event-storming, domain-storytelling, context-mapping, collaborative-modeling, workshop-facilitation, strategic-design]
source: GitHub
---

# DDD Toolbox - EventStorming and Domain Storytelling Strategic Design Tool

## What is it?
DDD Toolbox is an open-source, browser-based suite of strategic design tools built specifically for Domain-Driven Design (DDD) practitioners. It provides semantically-aware canvases for EventStorming, Domain Storytelling, and Context Mapping — the three core collaborative modeling techniques used to discover business domains and define system boundaries. Unlike generic diagramming tools, it understands DDD concepts natively and guides users through established practices.

## Why it matters for Business Analysts
BAs facilitating domain discovery workshops often resort to physical sticky notes or generic tools (Miro, Mural) that lack DDD semantics, making it harder to enforce consistent modeling conventions. DDD Toolbox fills this gap with purpose-built canvases that keep teams aligned on what each element means. EventStorming surfaces hidden business complexity and domain events that BAs can translate directly into requirements. Domain Storytelling creates shared understanding between business stakeholders and developers through visual narratives. Context Mapping clarifies integration boundaries and ownership, which is critical for large-scale requirements decomposition and stakeholder alignment.

## How to use it in BA Workflows
1. **Domain Discovery Workshops** - Run EventStorming sessions with stakeholders to identify domain events, commands, aggregates, and bounded contexts; the purpose-built canvas enforces correct DDD notation so output is immediately useful for developers and architects
2. **Business Process Narration** - Use Domain Storytelling canvases to capture how actors, work items, and systems interact in plain language, creating visual narratives that both business and IT stakeholders can validate and sign off on
3. **Requirements Scoping** - Leverage Context Map views to define integration points and ownership boundaries early in requirements gathering, preventing scope creep and surfacing cross-team dependencies
4. **Stakeholder Alignment Sessions** - Run iterative modeling sessions where business owners annotate domain stories with opacity highlighting during story playback, focusing discussion on specific process steps
5. **Handoff to Development Teams** - Export modeled domains and context maps as structured artifacts developers can use directly for bounded context design and API contract discussions

## Key Features
- Purpose-built EventStorming canvas with DDD-aware shape semantics (domain events, commands, policies, aggregates)
- Domain Storytelling modeler with icon-driven actors and work objects
- Context Mapping support for defining bounded contexts and integration relationships
- Story playback with opacity highlighting to walk through domain stories step by step
- Collaborative modeling interface designed for real-time workshop facilitation
- Open-source TypeScript codebase with active development since November 2024

## Technology Stack
- **Languages:** TypeScript
- **License:** Open Source (check repository for specific license)
- **Platform:** Browser-based, no install required

## GitHub Resources
- [poulainpi/ddd-toolbox](https://github.com/poulainpi/ddd-toolbox) - Strategic design tools for Domain-Driven Design featuring collaborative modeling and visual communication

## Related Skills
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Featmap - User Story Mapping]]
- [[Stakeholder Analysis Framework]]
