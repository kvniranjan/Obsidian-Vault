---
date: 2026-06-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, dmn, decision-management, decision-table, bpmn, process-modeling, decision-modeling]
source: GitHub
---

# dmn-js - Browser-Based DMN Decision Table Viewer and Editor

## What is it?
dmn-js is an open-source JavaScript toolkit from the bpmn-io team that allows users to view and edit DMN (Decision Model and Notation) diagrams and decision tables directly in the browser. It supports the full DMN 1.3 standard, including decision tables, decision requirement diagrams (DRDs), and literal expressions. The library is embeddable in any web application and serves as the DMN engine behind tools like Camunda Modeler.

## Why it matters for Business Analysts
DMN is the OMG standard for capturing and automating business decision logic, making dmn-js a natural fit for BAs who need to document and validate decision rules without writing code. It allows analysts to build decision tables that stakeholders can read, review, and sign off on — bridging the gap between business intent and technical implementation. The visual DRD editor helps BAs map out complex decision hierarchies, exposing dependencies between decisions that might otherwise be buried in requirements documents. Because it runs in the browser, it can be embedded in internal portals or documentation wikis, making decision models accessible to non-technical stakeholders.

## How to use it in BA Workflows
1. **Decision Logic Documentation** - Model business rules as DMN decision tables to replace ambiguous narrative text in requirements; each rule row becomes a traceable, testable acceptance criterion.
2. **Stakeholder Review of Business Rules** - Embed the dmn-js viewer in a lightweight web page and share it with business stakeholders for visual validation of decision logic before development begins.
3. **Decision Requirement Diagramming** - Use the DRD editor to map out how top-level business decisions depend on sub-decisions and input data, clarifying scope and data requirements early in analysis.
4. **Gap Analysis on Existing Rules** - Import existing DMN files from tools like Camunda or Drools into dmn-js to visualize and annotate gaps, contradictions, or missing conditions in rule sets.
5. **Regulatory Compliance Modeling** - Translate compliance rules (credit scoring, insurance underwriting, eligibility checks) into auditable DMN tables that demonstrate rule coverage to auditors and regulators.

## Key Features
- Full DMN 1.3 support including decision tables, DRDs, and literal expressions
- Editable and read-only viewer modes for both authoring and review use cases
- Hit policy support (UNIQUE, FIRST, COLLECT, RULE ORDER, etc.) matching OMG standard semantics
- Modular architecture — embed only the viewer, editor, or both
- Exports valid `.dmn` XML compatible with Camunda, Flowable, Drools, and other engines
- Extensible plugin API for custom renderers, linters, and overlays

## Technology Stack
- **Languages:** JavaScript (ES modules)
- **Dependencies:** diagram-js, min-dom, ids (all bpmn-io ecosystem)
- **License:** MIT

## GitHub Resources
- [bpmn-io/dmn-js](https://github.com/bpmn-io/dmn-js) - Browser toolkit for viewing and editing DMN decision models and tables

## Related Skills
- [[bpmn-io Web Modeler]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
