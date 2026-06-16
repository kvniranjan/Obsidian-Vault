---
date: 2026-06-16
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, workflow, diagramming, er-diagram, uml, flowchart, javascript, open-source]
source: GitHub
---

# LogicFlow - Business-Customizable Flow and Process Diagram Framework

## What is it?
LogicFlow is an open-source, highly customizable flowchart and process diagram editing framework from DiDi (the ride-hailing technology company), built with TypeScript. It provides an interactive rendering and editing engine for creating BPMN diagrams, ER diagrams, UML models, mind maps, workflow graphs, and custom business visualizations — all embeddable directly in web applications via React or Vue2 components. With over 11,000 GitHub stars, it is one of the most widely adopted open-source diagramming libraries focused specifically on business customization.

## Why it matters for Business Analysts
BAs must model and communicate complex processes, data structures, and decision logic to both technical and non-technical audiences — and LogicFlow covers all of these with a single framework. Its first-class BPMN 2.0 extension means BAs can produce standards-compliant process diagrams that integrate with workflow engines like Flowable or Camunda. The extensible node and edge plugin system lets teams define custom diagram vocabularies that match domain-specific business objects, reducing the translation gap between business models and technical specifications. Because it is an embeddable library rather than a locked SaaS tool, organisations can integrate it directly into internal portals, requirements wikis, or collaboration platforms, keeping process documentation co-located with other BA artefacts.

## How to use it in BA Workflows
1. **BPMN Process Modeling** - Use the built-in BPMN 2.0 extension to draw end-to-end business processes with standard swimlane notation; export the XML to hand off directly to workflow engine developers or import into Camunda Modeler for execution.
2. **ER Diagram for Data Requirements** - Leverage the ER diagram capability to document data entities, attributes, and relationships when eliciting data requirements, creating a shared model between BAs and data architects before any database design begins.
3. **Workflow and Approval Path Design** - Model multi-step approval workflows, escalation paths, and conditional branches as interactive diagrams; embed them in stakeholder review pages so business owners can validate routing logic without reading code or YAML.
4. **Custom Domain-Specific Diagrams** - Extend LogicFlow with bespoke node types and edge rules to represent proprietary business objects (e.g., insurance products, loan stages, logistics milestones), creating a visual language that speaks directly in business terms.
5. **Embedded BA Tooling Integration** - Integrate LogicFlow into internal requirements management portals or knowledge bases (e.g., alongside Confluence or Outline) so BAs can create and edit diagrams inline with written requirements, eliminating context-switching between tools.

## Key Features
- BPMN 2.0 official extension with standard shapes and XML import/export
- ER diagram and UML state-machine diagram support out of the box
- Plugin architecture for fully custom node types, edge types, and business rules
- React and Vue2 first-party wrappers for easy integration into modern front-ends
- SVG-based rendering enabling crisp, scalable exports
- Built-in undo/redo, zoom controls, grid, snap-to-grid, and minimap
- Layout algorithms supporting hierarchical, tree, and free-form arrangements
- Active maintenance with regular releases and a large Chinese enterprise community

## Technology Stack
- **Languages:** TypeScript, JavaScript
- **Dependencies:** React (optional extension) or Vue2 (optional extension); no heavy runtime dependencies
- **License:** Apache 2.0

## GitHub Resources
- [didi/LogicFlow](https://github.com/didi/LogicFlow) - Business-customizable flowchart editing framework supporting BPMN, ER, UML, and workflow diagrams

## Related Skills
- [[bpmn-io Web Modeler]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[BPMN Assistant (LLM-Powered)]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[TextUSM - Text-Based Diagram Generator]]
