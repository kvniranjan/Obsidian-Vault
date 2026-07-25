---
date: 2026-07-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, uml, sysml, c4, diagramming, ai-assisted, process-modeling, workflow-automation]
source: GitHub
---

# Drawio-Skill - AI-Powered Natural Language Diagram Generation

## What is it?
Drawio-Skill is a Claude Code skill (also compatible with Cursor, Copilot, and other agent frameworks) that generates professional draw.io diagrams from plain-English descriptions. It provides 11 diagram presets including BPMN, UML, SysML/MBSE, C4, and cross-functional swimlanes, with 36 tools covering everything from codebase-to-diagram conversion to image-to-editable-diagram transformation. Output is exported as native `.drawio` XML and optionally as PNG, SVG, PDF, or JPG.

## Why it matters for Business Analysts
BAs spend significant time creating and maintaining process diagrams, but traditional tools require manual drawing effort that slows down requirements workshops and stakeholder reviews. Drawio-Skill lets analysts describe a business process or system in plain language and receive a fully-structured, styled diagram immediately, dramatically reducing the time between discovery and documentation. It supports BPMN swimlane diagrams, decision flows, and entity-relationship diagrams that are core BA deliverables. The vision self-check capability means diagrams are validated against the draw.io shape library (10,000+ shapes including AWS, Azure, BPMN, UML), ensuring professional output without manual shape hunting.

## How to use it in BA Workflows
1. **Process Modeling from Meeting Notes** - After a requirements workshop, paste raw notes describing a business process and generate a BPMN swimlane diagram instantly, ready to share with stakeholders for validation.
2. **Current-State / Future-State Documentation** - Describe AS-IS and TO-BE processes in natural language and produce parallel diagrams for gap analysis presentations without opening a diagramming tool manually.
3. **System Context Diagrams (C4)** - Describe a system's actors and integrations verbally to generate C4 context or container diagrams for architecture review sessions.
4. **Reverse-Engineering Existing Systems** - Point the skill at a codebase, SQL schema, or Terraform/Kubernetes config to auto-generate data flow or infrastructure diagrams that inform requirements and dependency analysis.
5. **Stakeholder-Ready Presentations** - Use the exec-view compression tool to produce simplified, high-level versions of complex diagrams tailored for non-technical stakeholders, and export to PNG/PDF for decks.

## Key Features
- **11 diagram presets** — BPMN, UML Class, Sequence, Flowchart, C4, ERD, SysML, Network Topology, ML Architecture, Cross-Functional Swimlane, Mind Map
- **36 tools** — includes codebase-to-diagram, image-to-editable-diagram, PR diff bot, click-through runbooks, build-up animation
- **Vision self-check** — AI validates the generated diagram visually before returning it
- **10,000+ shapes** — full draw.io shape library including AWS, Azure, GCP, Cisco, Kubernetes, BPMN, and UML styles
- **Multiple export formats** — `.drawio` XML (editable), PNG, SVG, PDF, JPG
- **Agent-framework agnostic** — works with Claude Code, Cursor, Copilot, OpenClaw, Hermes, Codex

## Technology Stack
- **Languages:** Python
- **Dependencies:** draw.io desktop CLI, Claude Code (or compatible agent runtime)
- **License:** Not specified (check repository)

## GitHub Resources
- [Agents365-ai/drawio-skill](https://github.com/Agents365-ai/drawio-skill) - Generate draw.io diagrams from natural language with 11 presets (BPMN, UML, C4…) and 36 tools

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[Gaphor - Simple UML SysML and Requirements Modeling Tool]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[ProcessPiper - Python Library for Business Process Diagrams as Code]]
