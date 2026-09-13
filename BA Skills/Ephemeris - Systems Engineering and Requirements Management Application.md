---
date: 2026-09-13
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, traceability, systems-engineering, open-source]
source: GitHub
---

# Ephemeris - Systems Engineering and Requirements Management Application

## What is it?
Ephemeris is an open-source desktop application (built with NWjs) for system engineering and requirements management. It lets teams manage stakeholders, requirements, functions, and products in a single unified model and link them together, then generate diagrams, specifications, and schedules directly from those relationships.

## Why it matters for Business Analysts
Ephemeris covers two of the core pillars of BA work — requirements management and stakeholder analysis — in one connected model instead of separate spreadsheets and documents. Because stakeholders, requirements, functions, and products are all linked entities, a BA can trace a requirement back to the stakeholder who raised it and forward to the product component that satisfies it, producing an audit-ready traceability chain with far less manual upkeep. The built-in diagramming (ERDs, mind maps, project breakdown structures) and Gantt/Kanban views also mean a BA can move from elicitation to visualization to delivery tracking without switching tools.

## How to use it in BA Workflows
1. **Stakeholder Mapping** - Register stakeholders in the project model and link each one to the requirements, functions, or meetings they are associated with, giving a clear view of who owns or cares about what.
2. **Requirements Capture and Linking** - Record functional and non-functional requirements and connect them to the functions and products that realize them, forming a live requirements traceability matrix.
3. **Meeting-Driven Requirements Capture** - Use the meeting panel during elicitation sessions to log discussion points and convert them directly into tracked requirements and action items.
4. **Specification and Diagram Generation** - Auto-generate project breakdown structures, entity-relationship diagrams, mind maps, and interface matrices from the linked model to share with stakeholders and technical teams.
5. **Verification, Validation, and Delivery Tracking** - Run verification/validation checks against requirements, then plan and monitor delivery using the built-in Gantt chart and Kanban board views.

## Key Features
- Unified data model linking Stakeholders, Requirements, Functions, and Products
- Meeting panel for capturing requirements and actions during elicitation sessions
- Auto-generated diagrams: project breakdown structure, ERDs, mind maps, interface matrices
- Text-based specification generation from the project model
- Verification and validation (V&V) workflow support
- Gantt chart scheduling and capacity planning
- Kanban board for task organization
- ArchiMate file import and CSV import support for migrating existing project data
- Cross-platform desktop app (Windows/Mac/Linux) plus a hosted web demo for evaluation

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** npm, NWjs (desktop app runtime)
- **License:** MIT

## GitHub Resources
- [shuart/ephemeris](https://github.com/shuart/ephemeris) - System engineering and requirements management application

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[Stakeholder Analysis Framework]]
- [[CAIRIS - Security-Driven Requirements and Persona Modeling Platform]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
