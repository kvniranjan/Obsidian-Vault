---
date: 2026-07-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, plantuml, event-storming, c4-model, domain-storytelling, diagram-as-code, architecture, aws, azure]
source: GitHub
---

# plantuml-libs — PlantUML Libraries for EventStorming, C4 Model, and Domain Storytelling

## What is it?
plantuml-libs is a curated collection of PlantUML icon sets and diagram libraries that extends PlantUML with pre-built shapes for EventStorming, C4 Model, Domain Storytelling, AWS, Azure, and GCP cloud architectures. It also ships an NPM CLI tool to manage and render these libraries locally or in CI pipelines. Each library is versioned and can be imported via URL or local path, letting teams maintain consistent, reusable diagram assets across a project.

## Why it matters for Business Analysts
BAs routinely need to communicate complex domain models, cloud integrations, and business processes to diverse stakeholders — but building those diagrams from scratch is slow and inconsistent. plantuml-libs provides ready-made EventStorming notation (commands, events, aggregates, policies) and C4 Model shapes (persons, systems, containers, components) that align with well-established modelling conventions that both technical and non-technical audiences recognise. Domain Storytelling support enables BAs to capture end-to-end business workflows as visual narratives during workshop sessions. Since all diagrams live as code in plain text files, they integrate naturally with requirements documentation, ADRs, and version-controlled specification repositories.

## How to use it in BA Workflows
1. **EventStorming workshops** - Import the EventStorming library to produce sticky-note-style diagrams from workshop notes; share the `.puml` source alongside JIRA/Confluence pages so the model stays in sync with evolving domain knowledge.
2. **C4 architecture context diagrams** - Use the C4 library to draw System Context and Container diagrams that show how a proposed solution fits into the enterprise landscape; attach these to BRD or SAD documents as living diagrams updated via PR.
3. **Cloud integration mapping** - Use AWS/Azure/GCP icon libraries to map current-state and future-state integration architectures when documenting as-is/to-be process models or conducting gap analyses.
4. **Domain Storytelling narratives** - Capture user journey and process discovery sessions in Domain Story format to validate scope, identify actors, and reveal hidden business rules before writing formal requirements.
5. **Automated diagram generation in CI** - Embed the NPM CLI in a documentation pipeline so diagrams are always regenerated from source; ensures BA artefacts (context diagrams, process flows) never become stale compared to the code they describe.

## Key Features
- EventStorming library with commands, domain events, aggregates, policies, and read-model shapes
- C4 Model library (Context, Container, Component, Code) for architecture communication
- Domain Storytelling library for actor-and-work-object narratives
- AWS, Azure, and GCP icon libraries covering hundreds of service shapes
- NPM CLI (`@tmorin/plantuml-libs`) for local management and batch rendering
- Versioned releases — pin a library version in diagram headers to prevent drift
- MIT-licensed, with all libraries importable by URL for zero-install usage in online PlantUML editors

## Technology Stack
- **Languages:** TypeScript (CLI), PlantUML DSL
- **Dependencies:** Node.js, PlantUML (Java)
- **License:** MIT

## GitHub Resources
- [tmorin/plantuml-libs](https://github.com/tmorin/plantuml-libs) - PlantUML diagram libraries for EventStorming, C4 Model, domain storytelling, and cloud architectures

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Pumla - Systematic PlantUML Model Reuse for Architecture and Requirements Documentation]]
- [[DDD Toolbox - EventStorming and Domain Storytelling Strategic Design Tool]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
