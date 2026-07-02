---
date: 2026-07-02
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, personas, risk-analysis, security, usability, stakeholder-analysis, goal-modeling]
source: GitHub
---

# CAIRIS - Security-Driven Requirements and Persona Modeling Platform

## What is it?
CAIRIS (Computer Aided Integration of Requirements and Information Security) is an open-source Python platform for eliciting, specifying, and validating secure and usable systems. Built from the ground up to unify usability, requirements engineering, and security risk analysis in a single model, it lets analysts define goals, requirements, use cases, personas, and threats — all linked together. It is freely available under the Apache Software License.

## Why it matters for Business Analysts
CAIRIS addresses a gap that most requirements tools ignore: the intersection of what users need, what the system must do, and what can go wrong. BAs can model personas and realistic task flows alongside formal requirements, then automatically surface conflicts where usability and security goals clash. The platform generates 12 distinct visualisation views — from people and risks to requirements and architecture — giving stakeholders a tailored window into the same underlying model. This makes it especially valuable in regulated industries (finance, health, defence) where requirements must demonstrably trace back to user goals and risk controls.

## How to use it in BA Workflows
1. **Persona-Driven Requirements Elicitation** - Create data-driven personas that capture goals, motivations, and environment; link each persona to tasks and requirements so traceability from user need to specification is automatic.
2. **Goal and Obstacle Modelling (KAOS)** - Model high-level stakeholder goals, decompose them into sub-goals, and identify obstacles that threaten achievement — producing a requirements rationale artefact reviewable with stakeholders.
3. **Risk and Threat Analysis** - Enter assets, threats, vulnerabilities, and attack patterns; CAIRIS computes risk scores and highlights which requirements need security controls, bridging the gap between BA and security teams.
4. **Automatic Visualisation for Stakeholder Reviews** - Generate diagrams covering people, risks, requirements, architecture, and physical location views from one model to tailor presentations to different audiences without manual diagram maintenance.
5. **Traceability Audit** - Leverage built-in traceability links between goals, requirements, tasks, and risk elements to produce impact analysis when requirements change, supporting change-control and compliance reporting.

## Key Features
- **Unified Model** - Single data store connects personas, goals, requirements, use cases, risks, and architecture elements
- **KAOS Goal Modelling** - Formal goal and obstacle notation for structured requirements decomposition
- **12 Auto-Generated Views** - Contextual diagrams produced on demand without manual drawing
- **Persona Management** - Rich persona editor with environment contexts and characteristic statements
- **Security & Usability Integration** - First-class support for threat modelling alongside usability analysis
- **REST API** - Headless server mode enables integration with CI pipelines and other tools
- **Import / Export** - XML-based exchange format for sharing models across teams

## Technology Stack
- **Languages:** Python (backend), JavaScript (web UI)
- **Dependencies:** Flask, MySQL, Sphinx (docs)
- **License:** Apache 2.0

## GitHub Resources
- [cairis-platform/cairis](https://github.com/cairis-platform/cairis) - Open-source requirements, persona, and risk modelling platform

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[Sphinx-Needs - Docs-as-Code Requirements Management for Sphinx]]
- [[Stakeholder Analysis Framework]]
- [[Loomio - Collaborative Decision Making and Stakeholder Engagement Platform]]
