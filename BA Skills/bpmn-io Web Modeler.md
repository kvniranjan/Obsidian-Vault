---
date: 2026-03-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, diagramming]
source: GitHub
---

# bpmn.io Web Modeler

## What is it?
bpmn.io is an open-source toolkit and web-based modeler for creating, editing, and rendering BPMN 2.0 (Business Process Model and Notation) diagrams directly in the browser. Maintained by the bpmn-io organization on GitHub, it provides a suite of libraries including `bpmn-js` (BPMN modeler/viewer), `dmn-js` (Decision Model and Notation), and form building tools.

## Why it matters for Business Analysts
BPMN is the international standard for visually documenting business processes. BAs use it to map as-is and to-be processes, communicate workflows to stakeholders, and align technical teams with business requirements. bpmn.io provides a free, embeddable, standards-compliant modeler that works without vendor lock-in.

## How to use it in BA Workflows
1. **Process Discovery** — Use the online editor at bpmn.io to sketch out current-state (as-is) processes during discovery workshops.
2. **To-Be Design** — Model future-state processes after gap analysis, sharing diagrams as `.bpmn` XML files.
3. **Stakeholder Walkthroughs** — Export diagrams as SVG/PNG for presentations or embed them in Confluence/SharePoint pages.
4. **Integration** — Embed `bpmn-js` in internal web tools to allow business teams to view/annotate processes without installing software.
5. **Handoff to Dev** — BPMN 2.0 XML files exported from bpmn.io can be imported directly into workflow engines (Camunda, Activiti, Flowable).

## Key Features
- Full BPMN 2.0 standard compliance (pools, lanes, events, gateways, subprocesses)
- Browser-based — no installation required; works offline too via self-hosting
- Export to SVG, PNG, or BPMN 2.0 XML
- Embeddable `bpmn-js` library for custom web applications
- Companion tools: `dmn-js` for decision tables, `form-js` for form design
- Active open-source community with frequent releases

## GitHub Resources
- [bpmn-io organization](https://github.com/bpmn-io) — Parent org hosting all modeler libraries
- [bpmn-io/bpmn-js](https://github.com/bpmn-io/bpmn-js) — Core BPMN 2.0 modeler/viewer library
- [bpmn-io/awesome-bpmn-io](https://github.com/bpmn-io/awesome-bpmn-io) — Curated list of bpmn.io integrations and extensions

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[Featmap - User Story Mapping]]
- [[Stakeholder Analysis Framework]]
