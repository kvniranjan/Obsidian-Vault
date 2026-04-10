---
date: 2026-04-09
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, workflow, bpm, process-modeling, dmn, cmmn, automation]
source: GitHub
---

# Flowable Engine - BPMN and BPM Workflow Automation Platform

## What is it?
Flowable Engine is a compact, highly efficient, open-source Business Process Management (BPM) platform that executes industry-standard BPMN 2.0 (Business Process Model and Notation), DMN (Decision Model and Notation), and CMMN (Case Management Model and Notation) models. Written in Java and backed by over 9,000 GitHub stars, Flowable is designed for developers, system administrators, and business users who need to automate, monitor, and improve business processes.

At its core, Flowable provides three distinct engines — a BPMN process engine, a DMN decision engine, and a CMMN case engine — all of which can run independently or together. This makes it suitable for everything from simple approval workflows to complex, multi-department case management scenarios. The platform includes visual drag-and-drop modeling tools, a REST API for integration, and a web-based administration and monitoring UI.

More recently, Flowable has added AI-assisted modeling (generating workflows from natural language), a dedicated agent engine for multi-agent orchestration, and real-time AI assistance during process execution. This positions Flowable as a forward-looking platform where BAs can define process logic in standards-based notation and deploy it into production with minimal engineering overhead.

## Why it matters for Business Analysts
Flowable bridges the gap between process documentation and live process execution — a critical capability for BAs who want their models to directly drive system behavior rather than serve only as static documentation:

- **Process Modeling to Execution:** BPMN diagrams designed by a BA can be directly deployed and run by the Flowable engine, eliminating translation loss between the analyst's model and the developer's implementation.
- **Decision Logic with DMN:** BAs can define business rules and decision tables using the DMN standard, keeping decision logic explicit, auditable, and separate from process flow.
- **Case Management with CMMN:** Complex, unstructured work (e.g., customer onboarding, investigations) can be modeled using CMMN, supporting adaptive and knowledge-intensive processes that don't follow a fixed path.
- **Process Monitoring and Analysis:** Flowable's admin UI provides real-time visibility into active process instances, task assignments, and bottlenecks — giving BAs data to support continuous improvement.
- **AI-Assisted Workflow Design:** The 2025 releases introduced natural language-to-workflow generation and AI-assisted task completion, reducing the time to model first-draft process flows.

## How to use it in BA Workflows

### Designing and Deploying a Business Process
1. Use Flowable's web-based modeler (or any BPMN-compatible tool like bpmn.io) to draw the process as a BPMN 2.0 diagram.
2. Export the `.bpmn` XML file and deploy it to the Flowable engine via REST API or the admin console.
3. Trigger a process instance manually or via an API call to test the flow.
4. Monitor active instances in the Flowable admin UI and verify task routing matches your model.

### Modeling Decision Rules with DMN
1. Identify decision points in your BPMN model where business rules determine branching (e.g., approval thresholds, eligibility checks).
2. Create a DMN decision table in Flowable Modeler, defining input conditions and output values.
3. Reference the DMN table from the BPMN process using a Business Rule Task node.
4. Test the decision table with sample input data to verify all rule conditions behave as expected.

### Analyzing Process Performance
1. Run a set of representative process instances through the engine.
2. Open the Flowable admin UI and navigate to the process history view.
3. Review completed instances, average task durations, and any stuck or overdue tasks.
4. Use findings to identify bottlenecks and refine the BPMN model for the next iteration.

## Key Features
- Full BPMN 2.0, DMN 1.3, and CMMN 1.1 standards support
- Visual web-based process and decision modeler
- REST API for programmatic process control and integration
- Real-time monitoring dashboard for active and historical process instances
- Multi-agent orchestration support with dedicated AI agent engine (2025.1+)
- AI-assisted workflow generation from natural language descriptions
- Embeddable as a library in Spring Boot / Java applications
- 9,171 stars on GitHub | Apache-2.0 License | Actively maintained (2025 releases)

## Installation
```bash
# Run Flowable via Docker (quickest setup)
docker run -p 8080:8080 flowable/all-in-one

# Access at http://localhost:8080/flowable-ui
# Default credentials: admin / test

# Or add to a Maven project:
# <dependency>
#   <groupId>org.flowable</groupId>
#   <artifactId>flowable-spring-boot-starter</artifactId>
#   <version>7.x.x</version>
# </dependency>
```

## GitHub Resources
- [flowable/flowable-engine](https://github.com/flowable/flowable-engine) — Core BPMN, DMN, and CMMN workflow engine with REST API, modeler, and admin UI

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[dmnmd - DMN Decision Tables in Markdown]]
