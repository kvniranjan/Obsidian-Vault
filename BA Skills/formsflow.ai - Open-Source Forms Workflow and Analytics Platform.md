---
date: 2026-07-10
type: skill
category: Business Analysis
tags: [business-analyst, skill, bpmn, workflow-automation, forms, analytics, no-code, process-management, camunda, data-visualization]
source: GitHub
---

# formsflow.ai - Open-Source Forms Workflow and Analytics Platform

## What is it?
formsflow.ai is an open-source, low-code platform that integrates form building, BPMN workflow automation, and analytics into a single unified framework. It combines trusted open-source engines — form.io for forms, Camunda for workflow, Keycloak for security, and Redash for analytics — into one seamless deployment. The platform enables organizations to digitize and automate business processes without expensive enterprise software licensing.

## Why it matters for Business Analysts
BAs can design and deploy end-to-end digital processes — from intake form to approval workflow to outcome dashboard — entirely within one platform, without needing developers for routine process changes. The drag-and-drop form builder and BPMN workflow editor allow BAs to directly translate requirements into working solutions, closing the gap between analysis and delivery. The built-in analytics layer lets BAs track submission volumes, process cycle times, and bottlenecks to continuously improve workflows. As a viable open-source alternative to platforms like Microsoft Power Apps or ServiceNow, it gives BAs freedom to model complex, multi-step business processes with full auditability.

## How to use it in BA Workflows
1. **Digitize Paper or Email-Based Processes** - Use the form builder (powered by form.io) to design structured intake forms that replace unstructured email or paper submissions, capturing consistent data fields from requestors.
2. **Model Approval Workflows in BPMN** - Attach a Camunda BPMN process to any form so submissions automatically route to the right reviewers, with conditional branching based on form data (e.g., escalate if amount > $10,000).
3. **Build Process Analytics Dashboards** - Configure Redash-powered dashboards to visualize submission trends, approval rates, SLA compliance, and process bottlenecks — turning raw workflow data into BA-ready insights.
4. **Prototype and Validate Stakeholder Workflows** - Rapidly prototype digital workflows with stakeholders using the no-code interface, gather feedback on routing logic and form fields, and iterate before any code is written.
5. **Document and Communicate AS-IS / TO-BE Processes** - Use the embedded BPMN modeler to produce shareable process diagrams that can be exported and included in BRDs, process improvement reports, or stakeholder presentations.

## Key Features
- **Drag-and-Drop Form Builder** - form.io-powered designer supporting complex field types, conditional logic, and multi-page forms
- **BPMN Workflow Engine** - Camunda-backed process engine supporting parallel gateways, timers, service tasks, and human task assignment
- **Role-Based Access Control** - Keycloak integration for managing submitters, reviewers, approvers, and administrators
- **Analytics and Reporting** - Redash dashboards for real-time process metrics and form submission analysis
- **Docker-Based Deployment** - Full stack deployable via Docker Compose, suitable for self-hosted or cloud environments
- **Multi-Tenancy Support** - Supports multiple departments or teams within a single platform instance
- **API Integration** - REST APIs for connecting formsflow.ai processes to external systems and data sources

## Technology Stack
- **Languages:** JavaScript (React frontend), Python (API services), Java (Camunda workflow engine)
- **Dependencies:** form.io, Camunda BPM, Keycloak, Redash, PostgreSQL, Redis
- **License:** Apache 2.0

## GitHub Resources
- [AOT-Technologies/forms-flow-ai](https://github.com/AOT-Technologies/forms-flow-ai) - Core platform repository combining forms, workflow, and analytics

## Related Skills
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Activepieces - No-Code AI Workflow Automation Platform]]
- [[n8n - Fair-Code Workflow Automation Platform]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[Apache Superset - Data Exploration and Visualization Platform]]
