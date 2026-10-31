---
date: 2026-10-31
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, workflow-automation, low-code, forms]
source: GitHub
---

# Bonita Engine - Open-Source Low-Code BPMN Process and Forms Platform

## What is it?
Bonita Engine is the open-source core of the Bonita BPM platform, a Java-based runtime that deploys, executes, and manages process-based applications modeled in BPMN 2.0. It pairs with Bonita Studio, a low-code designer where business analysts model processes graphically and build the forms and UI screens that drive them, while developers extend the same project with code when needed.

## Why it matters for Business Analysts
Bonita is built around a BA-friendly division of labor: analysts own the BPMN process model and the forms/UI layer in a visual designer, while engineers handle deeper integrations and custom connectors in the same project. That means a BA can go from a mapped-out process to a working, form-driven application without waiting on a full development cycle for every change. Its Community (open-source) and Enterprise editions share the same modeling language, so proofs of concept built by a BA scale cleanly into production deployments. For analysts documenting "as-is" vs "to-be" workflows, Bonita doubles as both the modeling tool and the execution engine, closing the gap between process diagram and running system.

## How to use it in BA Workflows
1. **Process discovery to executable model** - Capture stakeholder workflows as BPMN 2.0 diagrams in Bonita Studio, then validate the model by running it directly rather than handing it off as a static diagram.
2. **Rapid form and UI prototyping** - Use the built-in form/UI designer to attach data-entry screens to each process step, letting BAs demo a working flow to stakeholders in the same session as the process walkthrough.
3. **Connector-driven integration mapping** - Document and wire up integrations to existing databases and systems via Bonita's connector framework, giving BAs a concrete artifact for "systems touched" sections of requirements docs.
4. **Iterative process governance** - Version and republish process definitions as requirements change, supporting ongoing BPM governance rather than one-off diagramming.
5. **Community-to-Enterprise handoff** - Prototype and pilot processes on the free Community edition, then present a working model as the business case for an Enterprise rollout with added monitoring and support.

## Key Features
- BPMN 2.0 compliant process engine with full execution semantics, not just diagramming
- Low-code Studio for process design, form building, and UI composition aimed at non-developers
- Connector framework for integrating external databases, APIs, and systems
- Clear low-code/pro-code split so BAs and developers can co-own the same project
- Open-source Community edition plus a commercial Enterprise edition with added capabilities

## Technology Stack
- **Languages:** Java
- **Dependencies:** Bonita Studio (low-code designer), Bonita Portal/UI runtime, standard BPMN 2.0 engine components
- **License:** GNU LGPL-2.1

## GitHub Resources
- [bonitasoft/bonita-engine](https://github.com/bonitasoft/bonita-engine) - Deploy, execute, and manage process-based applications built with Bonita Studio or the Engine APIs

## Related Skills
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[jBPM - Java Business Process Management Suite]]
- [[formsflow.ai - Open-Source Forms Workflow and Analytics Platform]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
