---
date: 2026-04-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-modeling, DMN, business-rules, decision-tables, automation]
source: GitHub
---

# GoRules Zen - Open-Source Business Rules Engine

## What is it?
**GoRules Zen** is an open-source, cross-platform Business Rules Engine (BRE) written in Rust, with native language bindings for NodeJS, Python, Go, Java, C#, Kotlin, and Swift. It enables organizations to define, manage, and execute complex business rules as structured decision models — without embedding logic deep in application code.

At its core, Zen uses a JSON Decision Model (JDM) format to represent decision graphs. Business rules are expressed as decision tables, expression nodes, and switch nodes — all composable into a visual graph that mirrors the logic a BA would draw on a whiteboard. An open-source React-based editor (JDM Editor) makes the graph visual and interactive.

With over 1,600 GitHub stars and active releases, Zen has strong community adoption and is used by teams needing auditable, version-controlled, and developer-handoff-ready business rules across diverse tech stacks.

## Why it matters for Business Analysts
Business rules — pricing tiers, eligibility criteria, risk classifications, approval thresholds — are often buried in code, spreadsheets, or undocumented system behavior. Zen gives BAs a structured, visual language to capture these rules in a form developers can execute directly.

- **Decision Tables:** Author structured rules using inputs, outputs, and conditions (equality, ranges, booleans, dates, arrays) in a tabular format — the same format BAs already use in BRDs and requirement specs.
- **Visual Decision Graphs:** Compose decision tables, expressions, and branching switch nodes into a flowchart-style graph, making complex logic readable by both business and technical stakeholders.
- **Multi-language Handoff:** Exported JDM files run natively in NodeJS, Python, Go, Java, C#, and more — removing translation overhead between BA deliverables and developer implementations.
- **Version Control Friendly:** Rules stored as JSON files integrate naturally into git, enabling change history, peer review via pull requests, and rollback — supporting governance and audit requirements.
- **Reusable Decision Nodes:** Sub-decisions can be referenced and composed, reducing duplication and aligning with modular requirements design principles.

## How to use it in BA Workflows

### Defining Eligibility Rules as a Decision Table
1. Identify the business rule: e.g., loan eligibility based on credit score and income tier.
2. Open the JDM Editor and create a Decision Table node.
3. Define input columns (Credit Score, Annual Income) and output column (Decision).
4. Add rows for each condition combination: `>= 750 → Approved`, `650-749 + income >= 50000 → Approved`, etc.
5. Export the JDM file and hand it off to developers for direct integration.

### Composing Multi-Step Decision Flows
1. Model each decision stage as a separate node (e.g., Risk Classification → Interest Rate Lookup → Final Offer).
2. Use Switch nodes to branch on intermediate outputs (e.g., "if Risk = High, route to Manual Review").
3. Connect nodes into a graph in the JDM Editor to represent the end-to-end business rule flow.
4. Validate the graph against sample inputs using the engine's evaluate API.

## Key Features
- Cross-platform BRE written in Rust with bindings for 8+ languages
- Decision Tables with support for ranges, booleans, date-time, and array conditions
- Switch nodes for conditional branching within a decision graph
- Expression nodes using the Zen Expression Language for data transformation
- Reusable Decision nodes to compose and reference sub-decisions
- Open-source React JDM Editor for visual rule authoring
- JSON-based JDM format — version-controllable and diff-friendly
- 1,600+ stars on GitHub | Apache 2.0 License | Actively maintained (2025)

## Installation
```bash
# NodeJS
npm install @gorules/zen-engine

# Python
pip install zen-engine

# Go
go get github.com/gorules/zen-go
```

## GitHub Resources
- [gorules/zen](https://github.com/gorules/zen) — Core Zen Business Rules Engine (Rust + multi-language bindings)

## Related Skills
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[bpmn-io Web Modeler]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
