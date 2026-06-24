---
date: 2026-06-24
type: skill
category: Business Analysis
tags: [business-analyst, skill, no-code, workflow-automation, data-modeling, ai-workflow, business-systems, low-code]
source: GitHub
---

# NocoBase - AI-Powered No-Code Business System Builder

## What is it?
NocoBase is an open-source, self-hosted AI + no-code platform for building custom business systems rapidly. Unlike form-driven tools, it uses a **data model-driven architecture** that separates the user interface from the data structure, enabling complex applications like CRMs, ERPs, approval systems, and custom BPM platforms. Its microkernel plugin architecture means every feature — from data sources to AI workflows — can be added or swapped as a plugin.

## Why it matters for Business Analysts
BAs frequently need to validate requirements by putting working prototypes in front of stakeholders, but building even lightweight apps traditionally requires developer time. NocoBase lets a BA independently build data models, configure permission structures, and wire approval workflows to demonstrate how a business system should behave — all without writing code. Its **AI Employees** feature lets embedded AI agents read the live data model and business context to assist with data entry, lookups, and task execution directly inside the system. This closes the loop between requirements discovery and rapid prototype validation in a single tool.

## How to use it in BA Workflows
1. **Requirements Prototyping** - Build a working prototype of the proposed system (tables, relationships, forms, and views) to walk stakeholders through concrete data flows and validate requirements before development starts.
2. **Approval Workflow Modeling** - Use the built-in workflow engine to model and test multi-step approval processes (e.g., change requests, sign-off chains), making the "as-should-be" process tangible for review.
3. **Data Model Validation** - Create entity-relationship structures visually and share them with domain experts to confirm data definitions, cardinalities, and business rules without needing a database diagram tool.
4. **Role and Permission Documentation** - Configure role-based access controls and field-level permissions to map out the authorization matrix, producing a living artifact that doubles as both a prototype and a specification.
5. **AI-Assisted Analysis** - Configure AI Employees to automate routine BA tasks inside the prototype — classifying incoming requests, generating summaries, or flagging missing fields — and demonstrate AI augmentation scenarios to stakeholders.

## Key Features
- **Data Model-Driven UI** - Separates data structure from interface, enabling complex system design without schema lock-in
- **Microkernel Plugin Architecture** - All capabilities (AI, auth, data sources, workflows) are individually loaded plugins, keeping the core lightweight and extensible
- **AI Employees** - AI agents embedded into the system that read the live data model and business context to perform tasks autonomously
- **Visual Workflow Engine** - Node-based workflow builder supporting triggers, conditions, approval steps, and AI nodes
- **Role-Based Permissions and Field Controls** - Fine-grained access model suitable for enterprise systems with multiple stakeholder groups
- **External Database and API Integration** - Connect to existing databases (PostgreSQL, MySQL, etc.) or REST APIs to build on real organizational data
- **WYSIWYG Interface Builder** - Drag-and-drop UI configuration without coding, making stakeholder demos easy to produce and iterate

## Technology Stack
- **Languages:** TypeScript, Node.js (backend), React (frontend)
- **Dependencies:** PostgreSQL or MySQL for storage; supports external API data sources
- **License:** Apache-2.0 (updated from AGPL-3.0 in February 2026)

## GitHub Resources
- [nocobase/nocobase](https://github.com/nocobase/nocobase) - Open-source AI + no-code platform for building business systems with data model-driven design and plugin extensibility

## Related Skills
- [[n8n - Fair-Code Workflow Automation Platform]]
- [[Activepieces - No-Code AI Workflow Automation Platform]]
- [[Dify - Production-Ready AI Agentic Workflow Platform]]
- [[Flowise - Visual AI Agent and Workflow Builder]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
