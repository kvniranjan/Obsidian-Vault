---
date: 2026-10-11
type: skill
category: Business Analysis
tags: [business-analyst, skill, enterprise-architecture, archimate, business-architecture, stakeholder-analysis, togaf]
source: GitHub
---

# Archi - Open Source ArchiMate Enterprise and Business Architecture Modeling Tool

## What is it?
Archi is a free, open-source, cross-platform tool for creating models in ArchiMate, the Open Group's independent enterprise architecture modelling language. It is built on the Eclipse Rich Client Platform in Java and is aligned with TOGAF, making it a low-cost entry point for individuals and organizations that want to model architecture without commercial tooling. Optional plugins extend it with Git-based collaborative modelling (coArchi) and JavaScript scripting for model automation and reporting (jArchi).

## Why it matters for Business Analysts
ArchiMate's Motivation layer gives BAs native modeling elements for Stakeholder, Driver, Assessment, Goal, Outcome, Requirement, and Constraint - letting stakeholder analysis and requirements traceability live in the same model as the business processes, capabilities, and application/technology layers they depend on. This connects BA artifacts (stakeholder maps, goal trees, requirements) directly to business process models, application landscapes, and technology, so impact analysis and change requests can be traced across layers rather than living in disconnected documents. Because it's free and standards-based, it's a practical way for BAs to learn or apply TOGAF/ArchiMate concepts without waiting on expensive enterprise architecture tooling procurement. The jArchi scripting plugin also opens the door to automating report generation, model validation, and bulk edits - useful for BAs maintaining large requirement or capability catalogs.

## How to use it in BA Workflows
1. **Stakeholder and Motivation Modeling** - Map Stakeholders, Drivers, Assessments, Goals, Outcomes, Requirements, and Constraints to formally capture "why" a change is needed and who cares about it, instead of a standalone stakeholder register.
2. **Business Process and Capability Mapping** - Model Business Layer elements (Business Process, Business Function, Business Service, Business Actor/Role) to document current-state ("as-is") and target-state ("to-be") operating models for a change initiative.
3. **Requirements Traceability Across Layers** - Link Requirement elements to the Business, Application, and Technology layer elements they affect, so a single model shows downstream impact when a requirement changes.
4. **Collaborative Modeling via coArchi** - Use the coArchi plugin to co-model with architects and other BAs through Git, enabling distributed teams to version and review architecture changes like code.
5. **Automated Reporting and Governance with jArchi** - Script bulk validation, naming-convention checks, or custom documentation exports (e.g., a requirements traceability matrix) directly from the model using jArchi's JavaScript API.

## Key Features
- Full ArchiMate 3.x notation support (Business, Application, Technology, Motivation, Strategy, Implementation & Migration layers)
- Free, cross-platform desktop tool (Windows, macOS, Linux) with no licensing cost
- coArchi plugin for Git-based collaborative/distributed model versioning
- jArchi plugin for JavaScript-based scripting, automation, and custom reporting
- Viewpoints and model views for tailoring diagrams to specific stakeholder audiences
- Model validation and element relationship checking aligned with the ArchiMate specification

## Technology Stack
- **Languages:** Java (Eclipse RCP application); JavaScript (jArchi scripting plugin)
- **Dependencies:** Eclipse Rich Client Platform; optional coArchi (Git) and jArchi plugins
- **License:** MIT

## GitHub Resources
- [archimatetool/archi](https://github.com/archimatetool/archi) - Free, open source, cross-platform ArchiMate modelling tool for enterprise and business architecture.

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Modelio - Open-Source Enterprise Architecture and BPMN Modeling Suite]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
