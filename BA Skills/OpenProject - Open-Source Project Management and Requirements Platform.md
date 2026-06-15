---
date: 2026-06-15
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, user-story-mapping, agile, project-management, stakeholder-analysis, roadmap, traceability]
source: GitHub
---

# OpenProject - Open-Source Project Management and Requirements Platform

## What is it?
OpenProject is the leading open-source web-based project management platform, supporting classical, agile, and hybrid project delivery from a single tool. It provides work packages (tasks, user stories, bugs, requirements, epics) with full traceability, Gantt charts, agile boards, roadmaps, wikis, and time/cost tracking. It is self-hostable under GPLv3 and widely adopted in enterprise and public-sector environments.

## Why it matters for Business Analysts
OpenProject gives BAs a structured, traceable environment to capture and manage requirements end-to-end — from discovery through delivery. Work packages support multiple types (user story, feature, bug, risk, change request) with custom fields, making it adaptable to any requirements framework without needing expensive commercial tools. Its Scrum and Kanban boards let BAs collaborate directly with development teams in the same system where requirements live, removing the handoff friction between analysis and delivery. The roadmap and version planning features enable BAs to communicate release scope and priority clearly to stakeholders.

## How to use it in BA Workflows
1. **Requirements Capture and Structuring** — Create work packages typed as "Requirements" or "User Stories," nest them under Epics, and assign attributes like priority, acceptance criteria, and status to build a structured, searchable requirements registry.
2. **Traceability and Impact Analysis** — Link work packages (relates to, duplicates, blocks, follows) to trace requirements through to implementation tasks and test cases, enabling rapid impact analysis when scope changes.
3. **Stakeholder Communication via Roadmap** — Use OpenProject's Roadmap view to show stakeholders which requirements are planned per release, communicating scope and sequencing without requiring access to internal backlogs.
4. **Agile BA Collaboration** — Maintain a sprint-ready backlog on Kanban or Scrum boards, participate in sprint planning with the development team, and update acceptance criteria and status in real time as stories are refined.
5. **Progress Reporting and Status Updates** — Use built-in dashboards, time-tracking, and budget modules to generate status reports for project sponsors, showing progress against planned scope and flagging risks or blockers.

## Key Features
- Work package types: tasks, user stories, epics, bugs, requirements, risks, change requests — all customizable
- Two-level hierarchy with projects and sub-projects for program-level requirements organization
- Gantt chart with dependencies and critical path for waterfall/hybrid delivery
- Scrum and Kanban boards with backlog and sprint management for agile delivery
- Roadmap view for release and version planning
- Traceability via work package relations (blocks, follows, relates to, duplicates)
- Wiki and document management for BA artifacts (BRDs, process docs, glossaries)
- Role-based access control and audit logs suitable for regulated industries
- REST API and GitHub/GitLab integration for dev-BA workflow alignment
- Self-hosted (Community Edition, GPLv3) or cloud-hosted (Enterprise)

## Technology Stack
- **Languages:** Ruby on Rails (backend), Angular (frontend), PostgreSQL
- **Dependencies:** Redis, Memcached, Nginx/Apache
- **License:** GPLv3 (Community Edition)

## GitHub Resources
- [opf/openproject](https://github.com/opf/openproject) - Full source code, issue tracker, and contribution guide for the leading open-source PM platform

## Related Skills
- [[OSRMT - Open Source Requirements Management Tool]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[Featmap - User Story Mapping]]
- [[Thunderdome - Agile Planning and Retro Suite]]
- [[Backlog.md - AI-Native Kanban and Task Management for Git]]
- [[Ploi Roadmap - Product Feedback and Roadmapping]]
