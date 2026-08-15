---
date: 2026-08-15
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, systems-engineering, traceability]
source: GitHub
---

# Ephemeris - System Engineering and Requirements Management Application

## What is it?
Ephemeris is an open-source system engineering and requirements management application that lets teams model stakeholders, requirements, functions, and products in one connected workspace. It combines a flexible entity/relation data model with visual editors — node graphs, ERDs, mindmaps, Gantt charts, and Kanban boards — so requirements and their traceability links stay visible alongside the rest of the project structure.

## Why it matters for Business Analysts
BAs are constantly asked to keep requirements, stakeholders, and deliverables traceable to each other as a project evolves, and most lightweight tools force a choice between spreadsheets (flexible but untraceable) and heavyweight enterprise requirements suites (traceable but rigid). Ephemeris lets a BA define a custom domain model, link stakeholders directly to the requirements and functions they own, and generate relationship graphs and breakdown structures automatically instead of maintaining them by hand. Built-in Verification & Validation (V&V) tracking and Gantt/capacity planning views mean a BA can manage the full requirements lifecycle — elicitation through V&V — without switching tools. Import support for Archimate and CSV also makes it easier to bring in existing enterprise architecture or legacy requirements data.

## How to use it in BA Workflows
1. **Stakeholder-to-requirement traceability** - Model stakeholders and link them directly to the requirements, functions, and products they care about, then auto-generate a relations graph to spot gaps or orphaned requirements.
2. **Requirements elicitation and structuring** - Capture requirements in text editors and create relations directly from the text, avoiding a separate manual linking step after elicitation sessions.
3. **Project breakdown and overview diagrams** - Build a project breakdown structure and let Ephemeris generate ERDs, mindmaps, and overview diagrams from the underlying relations for stakeholder presentations.
4. **Verification & Validation tracking** - Run V&V passes against requirements and functions to confirm coverage before sign-off, keeping an auditable trail of what was verified and when.
5. **Delivery planning** - Use the built-in Gantt charts, capacity planning, and Kanban "next actions" view to plan delivery of requirements alongside the traceability model, keeping planning and requirements data in sync.

## Key Features
- Custom domain modeling - define any model structure (not locked to a fixed requirements schema) to fit different BA/systems-engineering domains
- Node-based relation editor - draw relations visually or generate them from text, with automatic relation-graph generation
- Stakeholder, requirement, function, and product management in a single linked workspace
- Built-in V&V workflow for verification and validation sign-off
- Gantt charts, capacity planning, and Kanban views for delivery planning
- Archimate and CSV import for bringing in existing enterprise architecture or requirements data

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** Gulp (build), NW-Builder (desktop packaging)
- **License:** ISC

## GitHub Resources
- [shuart/ephemeris](https://github.com/shuart/ephemeris) - System engineering and requirements management application with stakeholder-to-requirement traceability

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Stakeholder Analysis Framework]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
