---
date: 2026-04-08
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, dmn, workflow-automation, process-modeling, low-code, citizen-developer, python]
source: GitHub
---

# SpiffArena - BPMN Workflow Automation Platform

## What is it?
SpiffArena is an open-source, low-code software development platform for building, running, and monitoring executable BPMN diagrams. Built on top of SpiffWorkflow — a mature Python BPMN 2.0 engine — it provides a full-stack web application with a visual BPMN/DMN editor, a process runner, and a monitoring dashboard, all accessible through a browser. Available at [github.com/sartography/spiff-arena](https://github.com/sartography/spiff-arena).

The platform is explicitly designed to empower "Citizen Developers" — business analysts, operations staff, and domain experts — to design and execute workflows without deep engineering involvement. Using BPMN flow charts and DMN decision tables, teams can capture complex business rules in a format that is both visually understandable and directly executable by the engine. This closes the gap between documentation and implementation that BAs often face.

SpiffArena supports the full BPMN 2.0 specification including call activities, sub-processes, message events, and timer events. Decision logic is modeled with DMN (Decision Model and Notation) tables embedded directly in process diagrams. Python scripts can be attached to tasks to handle data transformations or integrations, allowing BAs to delegate technical steps to developers while retaining full ownership of the process model.

## Why it matters for Business Analysts
SpiffArena bridges the traditional gap between BA process documentation and IT implementation — processes modeled by a BA can be deployed and executed directly, making the BA the author of running software:

- **Executable process models:** BPMN diagrams are not just documentation — they run on the SpiffWorkflow engine, eliminating the risk of implementation drift from the agreed process design.
- **DMN decision tables:** Business rules and decision logic are captured in readable DMN tables that analysts can own and update without coding, directly within the process diagram.
- **Citizen Developer empowerment:** The platform is deliberately built for non-developers; BAs can build, deploy, and iterate on workflows using the web UI without needing to touch application code.
- **Process monitoring and audit trails:** A built-in dashboard tracks active process instances, task statuses, and completion history — directly supporting audit, compliance, and performance reporting.
- **Human task management:** The platform supports human-in-the-loop tasks with forms, approvals, and notifications, making it suitable for approval workflows, change requests, and review cycles common in BA engagements.

## How to use it in BA Workflows

### Modeling and Deploying an Approval Workflow
1. Open the SpiffArena web editor and create a new BPMN process definition.
2. Draw swim lanes for each stakeholder role (Requestor, BA, Manager, IT).
3. Add User Tasks with web forms for each human step (e.g., submit request, BA review, manager approval).
4. Add a DMN Decision Task to encode approval routing rules (e.g., by cost threshold or risk level).
5. Deploy the process and share the task inbox URL with stakeholders for live execution.

### Embedding Business Rules with DMN Tables
1. Identify decision points in an existing BPMN process diagram (e.g., "eligibility check", "SLA tier assignment").
2. Create a DMN Decision Table task and define input/output columns matching your business variables.
3. Populate rows with the exact rule conditions from your BRD or business rules register.
4. Connect the DMN task to downstream BPMN flow so the output directly routes the process path.
5. Update the DMN table at any time without rewriting code — republish and the new rules take effect immediately.

### Monitoring and Reporting on Live Processes
1. Open the SpiffArena process monitoring dashboard.
2. Filter by process definition, date range, or task assignee to identify bottlenecks.
3. Export instance data to CSV for SLA analysis, cycle time reporting, or audit evidence.
4. Use monitoring data to drive AS-IS process analysis and identify improvement opportunities for TO-BE redesign.

## Key Features
- Full BPMN 2.0 support: tasks, gateways, events, sub-processes, call activities, message flows
- Integrated DMN decision table editor for business rule modeling
- Web-based drag-and-drop BPMN editor (no desktop install required)
- Python scripting support on script tasks for lightweight integrations and data transforms
- Human task inbox with web forms, assignees, and notifications
- Process instance monitoring dashboard with status tracking and audit history
- Docker Compose deployment for quick self-hosted setup
- ~130+ stars on GitHub | LGPL-2.1 License | Actively maintained (2025)

## Installation
```bash
# Clone the repository
git clone https://github.com/sartography/spiff-arena.git
cd spiff-arena

# Start all services with Docker Compose
docker compose up

# Access the web UI at http://localhost:7001
```

## GitHub Resources
- [sartography/spiff-arena](https://github.com/sartography/spiff-arena) — Full-stack SpiffWorkflow platform (editor + runner + monitor)
- [sartography/SpiffWorkflow](https://github.com/sartography/SpiffWorkflow) — Underlying Python BPMN 2.0 engine library

## Related Skills
- [[bpmn-io Web Modeler]]
- [[BPMN Assistant (LLM-Powered)]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
