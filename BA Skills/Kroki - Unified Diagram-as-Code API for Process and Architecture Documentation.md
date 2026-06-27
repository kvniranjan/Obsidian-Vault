---
date: 2026-06-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, diagrams-as-code, bpmn, process-modeling, documentation, architecture, uml, data-modeling]
source: GitHub
---

# Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation

## What is it?
Kroki is an open-source unified API that converts plain-text diagram descriptions into visual diagrams (SVG, PNG, PDF). It aggregates over 30 diagram tools — including BPMN, PlantUML, Mermaid, C4, ERD, Graphviz, Excalidraw, and UMLet — behind a single HTTP endpoint, so any text-capable environment (wikis, CI pipelines, Markdown docs) can render professional diagrams without installing separate toolchains.

## Why it matters for Business Analysts
BAs frequently switch between process diagrams (BPMN), architecture sketches (C4), data models (ERD), and sequence flows — each requiring a different tool. Kroki collapses all of these into one consistent API call, meaning diagrams live as version-controlled text alongside requirements documents and can be regenerated automatically. This eliminates the "stale diagram" problem where exported images fall out of sync with the underlying process. Kroki also integrates natively with Confluence, GitLab, GitHub, and Obsidian via plugins, embedding live diagrams directly into BA deliverables.

## How to use it in BA Workflows
1. **BPMN Process Documentation** - Write BPMN XML or use Mermaid flowchart syntax to describe as-is and to-be processes; submit to the Kroki API to generate publication-ready SVG diagrams for stakeholder review without a dedicated modeler application.
2. **System Context and Architecture Diagrams (C4)** - Use Structurizr DSL through Kroki to create C4 Level 1–3 diagrams (Context, Container, Component) that clearly show system boundaries and integration points for stakeholder discussions.
3. **Data Model Documentation** - Write ERD (Entity-Relationship Diagram) descriptions in plain text to generate data model visuals for data dictionary reviews, database design workshops, and integration mapping sessions.
4. **Sequence and Interaction Flows** - Use PlantUML or Mermaid sequence syntax to document how actors and systems interact across a business process, making handoff and integration requirements visually explicit.
5. **Living Documentation in Wikis** - Install the Kroki plugin for Confluence, GitLab, or Obsidian so that diagram code blocks inside BA documents render automatically, keeping all process visuals continuously up to date as requirements evolve.

## Key Features
- **30+ diagram types** — BPMN, C4, PlantUML, Mermaid, Graphviz, ERD, Excalidraw, UMLet, WaveDrom, BlockDiag, and more from a single endpoint
- **Self-hostable** — runs as a Docker container; no external SaaS dependency or data leaving your environment
- **Multiple output formats** — SVG (default), PNG, JPEG, and PDF for any stakeholder deliverable format
- **Encoding-based API** — diagram text is base64-encoded in the URL, making diagrams linkable and reproducible without a database
- **Plugin ecosystem** — native plugins for Confluence, GitLab, Asciidoctor, Obsidian, and more
- **Zero client-side tooling** — any HTTP client (curl, browser, Postman) can generate a diagram

## Technology Stack
- **Languages:** JavaScript, Java (server components)
- **Dependencies:** Docker (for self-hosting); individual diagram libraries bundled server-side
- **License:** MIT

## GitHub Resources
- [yuzutech/kroki](https://github.com/yuzutech/kroki) - Unified diagram-as-code API supporting 30+ diagram types from a single HTTP endpoint

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[TextUSM - Text-Based Diagram Generator]]
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
