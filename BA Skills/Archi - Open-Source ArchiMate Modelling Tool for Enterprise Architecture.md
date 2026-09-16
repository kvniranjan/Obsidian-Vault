---
date: 2026-09-16
type: skill
category: Business Analysis
tags: [business-analyst, skill, archimate, togaf, enterprise-architecture, modeling, process-modeling, capability-mapping]
source: GitHub
---

# Archi - Open-Source ArchiMate Modelling Tool for Enterprise Architecture

## What is it?
Archi is a free, cross-platform desktop tool for creating ArchiMate models — the open standard notation for describing business, application, and technology architectures. Built on the Eclipse RCP framework, it has been the de facto free entry point into ArchiMate modeling for over a decade, with a mature plugin ecosystem (including coArchi for Git-based collaboration) and strong TOGAF alignment.

## Why it matters for Business Analysts
Archi lets BAs model the business layer — business processes, functions, services, actors, and roles — and connect it explicitly to the application and technology layers that support it, which BPMN tools alone don't capture. This is essential when a BA needs to show how a proposed process change ripples into supporting systems and infrastructure, or when contributing to an architecture review board under a TOGAF ADM cycle. Because it's free and self-hostable, BAs on cost-constrained engagements can produce enterprise-grade architecture artifacts without waiting on an EA team's paid tooling. The coArchi plugin also lets multiple analysts collaborate on the same model via Git, which fits naturally into vault- and repo-based BA documentation practices.

## How to use it in BA Workflows
1. **Business Capability Mapping** - Model business capabilities, functions, and services as ArchiMate business-layer elements to give stakeholders a shared, structured view of "what the business does," independent of current org structure or systems.
2. **Current-State (Baseline) vs Target-State Architecture** - Build baseline and target ArchiMate views to communicate transformation roadmaps, showing how business processes, applications, and infrastructure evolve together during a change initiative.
3. **Process-to-System Traceability** - Link business processes and services to the application components and technology nodes that realize them, supporting impact analysis when a system change or migration is proposed.
4. **Stakeholder and Actor Modeling** - Use business actor, role, and collaboration elements to document who performs which process steps, complementing RACI matrices and stakeholder analysis artifacts.
5. **Architecture Governance Deliverables** - Export views to image or model-exchange formats for architecture review boards, and use coArchi to version-control models alongside requirements and process documentation in Git.

## Key Features
- Full ArchiMate 3.x notation support across business, application, technology, motivation, strategy, and implementation layers
- Model tree and multiple view canvases for organizing large, multi-domain architectures
- coArchi plugin for Git-backed collaborative modeling and model merging
- Model Exchange File format (Open Group standard) for interoperability with other ArchiMate tools
- Validation and model-checking to catch inconsistent or orphaned relationships
- Extensible plugin architecture (jArchi scripting for automation and bulk model edits)
- Active, long-running open-source project with regular releases

## Technology Stack
- **Languages:** Java
- **Dependencies:** Eclipse RCP platform
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Open-source ArchiMate modelling tool for enterprise, business, and technology architecture

## Related Skills
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[Stakeholder Analysis Framework]]
- [[PM Tools Templates - Comprehensive BA Template Library]]
