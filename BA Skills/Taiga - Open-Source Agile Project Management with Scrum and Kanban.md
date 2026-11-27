---
date: 2026-11-27
type: skill
category: Business Analysis
tags: [business-analyst, skill, agile, scrum, kanban, backlog-management, user-stories, project-management]
source: GitHub
---

# Taiga - Open-Source Agile Project Management with Scrum and Kanban

## What is it?
Taiga is a free and open-source agile project management platform that supports both Scrum and Kanban workflows in one workspace. It organizes epics, user stories, tasks, issues, sprints, and backlogs, and ships as a self-hostable stack (backend, frontend, and a Docker Compose deployment) under the MPL-2.0 license.

## Why it matters for Business Analysts
Taiga gives BAs a lightweight, self-hosted home for the artifacts they already produce — epics, user stories with acceptance criteria, and a prioritized backlog — without the licensing cost or complexity of heavier ALM suites. Its dual Scrum/Kanban boards let a BA model discovery-to-delivery flow (intake → refinement → sprint commitment) and track swimlanes, WIP limits, and sprint burndown directly against the requirements they authored. Built-in wiki pages let BAs attach supporting documentation (process notes, acceptance criteria, stakeholder decisions) next to the backlog items they describe, and GitHub/GitLab/Jira/Trello importers ease migration from existing trackers.

## How to use it in BA Workflows
1. **Backlog authoring** - Capture requirements as epics broken into user stories with descriptions, acceptance criteria, and story-point estimates, keeping the product backlog as the single source of truth for scope.
2. **Sprint and release planning** - Use the Scrum board to plan sprints, assign user stories to sprints, and track a project doom-line / burndown so BAs can communicate delivery risk to stakeholders.
3. **Process and intake modeling** - Use Kanban boards with custom swimlanes and WIP limits to model intake or change-request workflows (e.g., "Requested → Analysis → Ready for Dev → Done") separate from delivery sprints.
4. **Requirements documentation** - Use the per-project wiki to host supporting BA artifacts (business rules, glossary, decision logs) linked from the user stories that depend on them.
5. **Migration and stakeholder onboarding** - Import existing backlogs from GitHub, GitLab, Jira, or Trello to consolidate requirements history when standing up a new project space for stakeholders.

## Key Features
- Combined Scrum and Kanban templates usable per project or together
- Epics, user stories, tasks, and issues with role-based estimation
- Sprint task board with per-story swimlanes and sprint burndown/doom-line
- Customizable Kanban boards with WIP limits and filtering
- Built-in project wiki for supporting documentation
- Importers for GitHub, Jira, GitLab, and Trello; Slack and OAuth integrations
- Self-hostable via Docker Compose, or available as a hosted SaaS

## Technology Stack
- **Languages:** Python (backend, Django-based), CoffeeScript/TypeScript (frontend)
- **Dependencies:** Docker & Docker Compose for self-hosted deployment; PostgreSQL, RabbitMQ
- **License:** MPL-2.0 (backend); AGPL-3.0 (frontend)

## GitHub Resources
- [taigaio/taiga-docker](https://github.com/taigaio/taiga-docker) - Docker Compose deployment for self-hosting Taiga (2.2k stars)
- [taigaio/taiga-back](https://github.com/taigaio/taiga-back) - Taiga backend API (Python/Django)
- [taigaio/taiga-front](https://github.com/taigaio/taiga-front) - Taiga frontend application

## Related Skills
- [[Thunderdome - Agile Planning and Retro Suite]]
- [[Plane - Open-Source Agile Project Management and Requirements Platform]]
- [[OpenProject - Open-Source Project Management and Requirements Platform]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
- [[Featmap - User Story Mapping]]
