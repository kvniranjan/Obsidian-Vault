---
date: 2026-08-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, diagramming, ai-assisted, draw-io, process-modeling, workflow]
source: GitHub
---

# Drawio-AI-Kit - AI-Powered Draw.io Diagram Generation with BPMN Support

## What is it?
drawio-ai-kit is an open-source JavaScript toolkit that teaches AI agents to generate correct, beautiful draw.io diagrams using a declarative layout engine, ground-truth stencils, structural validator, and vision-based self-correction loop. It supports five diagram domains out of the box: AWS, Azure, GCP, Databricks, and BPMN. It integrates with AI coding agents (Claude Code, Codex, Gemini CLI) with zero external dependencies.

## Why it matters for Business Analysts
Business analysts spend significant time creating process diagrams manually — drawio-ai-kit lets AI agents generate structurally accurate BPMN diagrams from natural language descriptions or process narratives, cutting diagram creation time dramatically. The vision self-check loop means the AI validates its own output against BPMN rules before presenting results, reducing review cycles. Because it outputs native draw.io XML, diagrams are immediately editable in draw.io or diagrams.net, preserving the BA's usual tooling. It bridges the gap between AI-generated drafts and production-quality business process documentation.

## How to use it in BA Workflows
1. **BPMN Process Drafting** - Describe a business process in plain English to your AI agent; the kit's BPMN domain skill generates a compliant BPMN 2.0 diagram in draw.io format, ready for stakeholder review and iteration.
2. **Architecture and Context Diagrams** - Use the AWS, Azure, or GCP domain skills to rapidly produce system context diagrams that accompany BRDs and functional specifications, showing how a solution integrates with existing infrastructure.
3. **Iterative Process Refinement** - Leverage the render-analyze-rectify loop to have the AI automatically correct layout errors, overlap, and structural violations, so BAs spend time on content rather than formatting.
4. **Standardised Stencil Libraries** - Ground-truth stencils ensure generated diagrams use the same shapes and notation as enterprise draw.io standards, making outputs consistent across BA deliverables without manual template management.
5. **AI Agent Integration for BA Toolchains** - Install the CLI into a Claude Code or Gemini CLI session and invoke it inline during requirements workshops to produce live process diagrams from real-time discussion notes.

## Key Features
- Declarative layout engine — defines diagram structure via a logical spec, not pixel coordinates, reducing layout errors
- Ground-truth stencil registry — ensures correct shape usage for AWS, Azure, GCP, Databricks, and BPMN notation
- Structural validator — checks generated XML against domain rules before output
- Vision self-check — uses AI vision to inspect the rendered diagram and trigger correction if issues are detected
- Multi-agent support — auto-detects Claude Code, Codex, Gemini CLI, and other AI agents at install time
- Zero dependencies — lightweight install with no external runtime requirements beyond Node.js
- BPMN domain skill — full support for BPMN 2.0 notation including pools, lanes, gateways, events, and tasks

## Technology Stack
- **Languages:** JavaScript
- **Dependencies:** Zero runtime dependencies (Node.js required for CLI)
- **License:** MIT

## GitHub Resources
- [sparklabx/drawio-ai-kit](https://github.com/sparklabx/drawio-ai-kit) - Declarative AI diagramming kit for draw.io with BPMN, AWS, Azure, GCP, and Databricks domain skills

## Related Skills
- [[Drawio-Skill - AI-Powered Natural Language Diagram Generation]]
- [[BPMN Process Designer - Vue.js Extended BPMN Modeler Built on bpmn-js]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[Kroki - Unified Diagram-as-Code API for Process and Architecture Documentation]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
- [[LogicFlow - Business-Customizable Flow and Process Diagram Framework]]
