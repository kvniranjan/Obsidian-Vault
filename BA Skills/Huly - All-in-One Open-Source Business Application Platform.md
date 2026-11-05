---
date: 2026-11-05
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, stakeholder-analysis, project-management, collaboration]
source: GitHub
---

# Huly - All-in-One Open-Source Business Application Platform

## What is it?
Huly (hcengineering/platform) is an open-source framework for building and self-hosting business applications, bundling Issue Tracker, Project Management, Collaborative Documents, Team Chat, CRM, HRM, and an ATS into a single workspace. It is positioned as a self-hostable, open-source alternative to combining Linear, Notion, Slack, and Jira, and is licensed under the Eclipse Public License 2.0.

## Why it matters for Business Analysts
BAs constantly juggle requirements documents, stakeholder conversations, and delivery tracking across separate tools, which fragments traceability between a requirement, the discussion that shaped it, and the work item that implements it. Huly keeps documents, chat threads, and the issue tracker in one workspace with full-text search and an activity feed on every object, so a BA can trace a decision from stakeholder discussion to written requirement to tracked task without hopping tools. Because it is self-hostable and open source, organizations with data-residency or compliance constraints can run their own BA workspace rather than depending on a SaaS vendor.

## How to use it in BA Workflows
1. **Requirements documentation** - Use the built-in collaborative Documents app to draft and co-edit BRDs, user stories, and acceptance criteria with live multi-user editing, keeping requirements versioned alongside the rest of the project.
2. **Stakeholder communication capture** - Use Team Chat with threads and per-object activity feeds to keep stakeholder discussions attached directly to the requirement, issue, or milestone they relate to, preserving decision rationale for audits.
3. **Backlog and milestone tracking** - Use the Tracker (projects, components, milestones, sub-issues) to break epics into user stories and manage delivery progress visible to both BAs and engineering.
4. **Cross-artifact traceability** - Rely on platform-wide full-text search across issues, documents, and attachments to quickly trace which requirement drove which implementation task during impact analysis or change requests.
5. **Stakeholder relationship management** - Use the built-in CRM and HRM modules to track external stakeholder contacts and internal resourcing, useful for BAs managing stakeholder analysis across larger programs.

## Key Features
- Unified workspace combining issue tracking, documents, chat, CRM, HRM, and ATS
- Live collaborative document editing for requirements and specs
- Full-text search across issues, documents, and attachments
- Self-hostable via Docker Compose (or a dedicated huly-selfhost repo) for data control
- Typed API client for building custom integrations with other BA tooling

## Technology Stack
- **Languages:** TypeScript
- **Dependencies:** Docker Compose (self-hosted deployment), Node.js runtime
- **License:** Eclipse Public License 2.0 (EPL-2.0)

## GitHub Resources
- [hcengineering/platform](https://github.com/hcengineering/platform) - Open-source all-in-one business application platform (Tracker, Documents, Chat, CRM, HRM, ATS)

## Related Skills
- [[OpenProject - Open-Source Project Management and Requirements Platform]]
- [[Plane - Open-Source Agile Project Management and Requirements Platform]]
- [[Loomio - Collaborative Decision Making and Stakeholder Engagement Platform]]
- [[NocoBase - AI-Powered No-Code Business System Builder]]
