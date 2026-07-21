---
date: 2026-07-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, diagrams-as-code, python, flowchart, business-process]
source: GitHub
---

# ProcessPiper - Python Library for Business Process Diagrams as Code

## What is it?
ProcessPiper is an open-source Python library that generates business process diagrams — including BPMN-style flowcharts — from plain text or Python code. Rather than using a drag-and-drop GUI, analysts describe process flows programmatically, and the library renders professional-quality PNG diagrams. It supports swim lanes, events, tasks, gateways, and connectors covering the core visual vocabulary of business process documentation.

## Why it matters for Business Analysts
Business Analysts frequently need to document and share process flows, but maintaining diagram files in proprietary GUI tools creates versioning friction and collaboration barriers. ProcessPiper enables a diagrams-as-code approach where process documentation lives in text files that are diff-able, reviewable, and committable to version control alongside project artefacts. It integrates naturally with AI-assisted workflows — an LLM can generate or modify the plain-text process description, and ProcessPiper renders the output. It lowers the barrier to producing consistent, reusable process diagrams without requiring a licensed desktop tool.

## How to use it in BA Workflows
1. **As-Is Process Documentation** - Describe the current state of a business process as a series of pools, lanes, tasks, and gateways in plain text; ProcessPiper renders a professional swim-lane diagram that can be embedded in requirements documents or shared with stakeholders.
2. **To-Be Process Design** - Rapidly prototype alternative future-state process designs by editing the text definition and regenerating the diagram, enabling fast iteration during workshops without waiting for a modeller to redraw diagrams manually.
3. **AI-Augmented Process Generation** - Pass a process description or meeting transcript to an LLM and ask it to produce a ProcessPiper script; review and adjust the code output, then render the final diagram — accelerating documentation of processes captured during stakeholder interviews.
4. **Version-Controlled Process Libraries** - Store process definitions as `.py` or plain-text files in a Git repository alongside requirements and user stories, giving the team a single source of truth with full change history and PR-based review of process changes.
5. **Automated Documentation Pipelines** - Integrate ProcessPiper into CI/CD or documentation build pipelines (e.g. Sphinx, MkDocs) so that process diagrams are regenerated automatically whenever the source definition changes, keeping published documentation always current.

## Key Features
- **Swim-lane diagrams** - Supports pools and lanes for cross-functional process documentation
- **BPMN-inspired notation** - Tasks, events (start/end/intermediate), and gateways (exclusive, parallel) map to standard BPMN concepts
- **Plain-text syntax** - Process flows can be defined in a readable, indented text format without writing Python boilerplate
- **PNG output** - Renders diagrams to image files suitable for embedding in documents, wikis, or slide decks
- **Python API** - Full programmatic control for generating diagrams dynamically from data or templates
- **Zero GUI dependency** - Runs headlessly in scripts, notebooks, or automated pipelines

## Technology Stack
- **Languages:** Python
- **Dependencies:** Pillow (image rendering)
- **License:** MIT

## GitHub Resources
- [csgoh/processpiper](https://github.com/csgoh/processpiper) - Open source Python library to generate business process diagrams using code or plain text

## Related Skills
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[bpmn-io Web Modeler]]
- [[Egon.io - Domain Story Modeler for Collaborative Business Process Discovery]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
