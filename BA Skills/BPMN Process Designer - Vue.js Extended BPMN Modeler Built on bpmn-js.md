---
date: 2026-07-31
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, process-modeling, vue, workflow, diagram, open-source]
source: GitHub
---

# BPMN Process Designer - Vue.js Extended BPMN Modeler Built on bpmn-js

## What is it?
BPMN Process Designer is an open-source Vue.js component library that wraps and extends the industry-standard bpmn-js toolkit, providing a production-ready embeddable BPMN 2.0 modeler for web applications. It offers a rich UI layer on top of bpmn-js — including custom property panels, palette extensions, and localization — so teams can embed a full BPMN editing experience without building it from scratch. The project is widely used in enterprise internal portals and low-code platforms across the Chinese-speaking developer community, with nearly 1,800 stars on GitHub.

## Why it matters for Business Analysts
BAs often need to share and collaborate on BPMN process diagrams within internal web portals, approval systems, or low-code platforms — contexts where a standalone desktop tool is impractical. This library lets development teams quickly embed a browser-based BPMN editor that BAs can use without leaving the business system. Its extended property panel exposes flow metadata (task assignees, timers, conditions) directly in the UI, bridging the gap between a BA's process model and the technical execution configuration a developer needs. Because it is built on bpmn-js, any diagram created is fully BPMN 2.0 compliant and portable to other standards-based tools like Camunda, Activiti, or Flowable. For BAs working in agile delivery teams, having the modeler embedded in the project management or ticketing platform reduces the friction of switching contexts when documenting or refining process flows.

## How to use it in BA Workflows
1. **Embed in an internal process portal** - Work with your development team to install the Vue component into your organization's intranet portal, giving non-technical stakeholders a browser-based BPMN editor alongside project dashboards rather than requiring a separate desktop install.
2. **Model and export executable BPMN** - Use the extended modeler to draw end-to-end process flows with swim lanes, gateways, and task assignments, then export the `.bpmn` XML for direct import into Camunda, Flowable, or Activiti for process execution.
3. **Customize property panels for domain metadata** - Collaborate with developers to add custom fields (e.g., SLA, system owner, data classification) to the built-in property panel, so each BPMN element captures the business metadata BAs need without manual documentation side-cars.
4. **Localized stakeholder walkthroughs** - Leverage the library's localization support to deliver process walkthrough sessions in stakeholder-preferred languages, reducing the cognitive overhead of reading BPMN labels in a foreign language during facilitated workshops.
5. **Low-code platform integration** - For organizations building or maintaining a low-code workflow builder, use this component as the visual process design layer, giving BAs a drag-and-drop BPMN canvas that directly feeds workflow engine configurations without any code.

## Key Features
- Full BPMN 2.0 editing canvas built on bpmn-js with drag-and-drop palette
- Extended property panel with configurable fields for task metadata, execution listeners, and form keys
- Vue 2 / Vue 3 support with TypeScript declarations
- Localization (i18n) support for multilingual deployments
- Custom element rendering and palette plugin hooks for domain-specific extensions
- Import/export of BPMN 2.0 XML compatible with major BPM engines
- Demo pages illustrating integration patterns for common enterprise use cases

## Technology Stack
- **Languages:** TypeScript, JavaScript, Vue.js (Vue 2 and Vue 3)
- **Dependencies:** bpmn-js, diagram-js, bpmn-moddle, Vue 3 Composition API
- **License:** Apache License 2.0

## GitHub Resources
- [miyuesc/bpmn-process-designer](https://github.com/miyuesc/bpmn-process-designer) - Extended Vue.js BPMN modeler component built on bpmn-js for embedding in enterprise web apps

## Related Skills
- [[bpmn-io Web Modeler]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Camunda Modeler - Desktop BPMN DMN and Forms Modeling Tool]]
- [[Open-BPMN - Extensible BPMN 2.0 Modeler for IDEs and Web]]
- [[LogicFlow - Business-Customizable Flow and Process Diagram Framework]]
- [[SpiffWorkflow - Pure Python BPMN Workflow Engine]]
