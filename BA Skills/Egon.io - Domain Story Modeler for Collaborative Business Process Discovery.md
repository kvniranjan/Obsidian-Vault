---
date: 2026-07-14
type: skill
category: Business Analysis
tags: [business-analyst, skill, domain-storytelling, process-modeling, stakeholder-analysis, requirements-elicitation, domain-driven-design, collaboration, workshop-facilitation]
source: GitHub
---

# Egon.io — Domain Story Modeler for Collaborative Business Process Discovery

## What is it?
Egon.io is an open-source, browser-based tool for creating Domain Story diagrams — a visual language in which domain experts and developers jointly narrate how a business works using actors, work objects, and activities. Running entirely in the browser with no login required, it produces clear pictographic diagrams from collaborative workshops that capture business processes in a form both technical and non-technical stakeholders can immediately understand.

## Why it matters for Business Analysts
Domain Storytelling is a structured elicitation technique that cuts through ambiguity by having stakeholders literally tell stories about their work while the BA models the flow in real time. Egon.io makes that process fast and frictionless — the resulting diagrams double as both requirements artifacts and communication tools. Because the notation is pictographic rather than formal (no swim lanes or BPMN symbols to explain), stakeholders stay engaged and can self-validate the model on the spot. The tool also supports scope boundaries and domain-specific icon sets, giving BAs a lightweight way to define bounded contexts before moving into detailed requirements.

## How to use it in BA Workflows
1. **As-Is Process Discovery** — Run a facilitated workshop where domain experts narrate a typical day or scenario; model each step live in Egon.io while participants correct and enrich the story. Export the finished diagram as PNG or SVG for inclusion in BRDs and workshop reports.
2. **To-Be Process Design** — After capturing the current state, re-run the story with proposed changes, annotating differences with annotation bubbles. Side-by-side as-is and to-be diagrams make gap analysis concrete and stakeholder-reviewable.
3. **Requirements Elicitation and Scoping** — Use scope boundaries in Egon.io to draw system boundaries, clearly distinguishing what is in scope from what the system communicates with externally — directly feeding into context diagrams and system scope statements.
4. **Stakeholder Onboarding and Knowledge Transfer** — Share exported domain stories as living documentation that explains the business domain to new team members, developers, or auditors without requiring any domain expertise to read.
5. **DDD Bounded Context Discovery** — Use domain stories as a precursor to Context Mapper or similar DDD tools: the actors and work objects in a story naturally surface bounded contexts, ubiquitous language terms, and team responsibilities for strategic design workshops.

## Key Features
- Pictographic Domain Story notation (actors, work objects, activities, sequence numbers, annotations)
- Scope boundary overlays to visually define system perimeters
- Domain-specific icon sets — customise icons to match industry or team vocabulary
- Export to PNG, SVG, and DST (JSON) for documentation and version control
- Import/export DST files for sharing and asynchronous collaboration
- Replay mode to walk through a story step by step in presentations
- Runs fully in-browser — no install, no account, no server dependency
- Self-hostable via Docker or static file deployment for org-wide rollout

## Technology Stack
- **Languages:** TypeScript, JavaScript
- **Framework:** Angular
- **Dependencies:** bpmn.io toolkit (bpmn-moddle), Node.js build toolchain
- **License:** GNU General Public License v3.0

## GitHub Resources
- [WPS/egon.io](https://github.com/WPS/egon.io) — Browser-based Domain Story Modeler (826+ stars, actively maintained)

## Related Skills
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Featmap - User Story Mapping]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
- [[Stakeholder Analysis Framework]]
- [[bpmn-io Web Modeler]]
- [[TextUSM - Text-Based Diagram Generator]]
- [[Loomio - Collaborative Decision Making and Stakeholder Engagement Platform]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
