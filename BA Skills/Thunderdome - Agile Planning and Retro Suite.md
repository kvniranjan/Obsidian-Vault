---
date: 2026-03-24
type: skill
category: Business Analysis
tags: [business-analyst, skill, agile, planning-poker, retrospective, story-mapping, estimation, collaboration]
source: GitHub
---

# Thunderdome - Agile Planning and Retro Suite

## What is it?
Thunderdome is an open source, self-hostable agile collaboration platform built for remote and distributed teams. It combines **Planning Poker** (story point estimation), **Sprint Retrospectives**, **User Story Mapping**, and **Async Daily Standups** in a single tool. It is actively maintained on GitHub and available as a free hosted service or a Docker-deployed instance.

## Why it matters for Business Analysts
BAs are often the facilitators and note-takers in agile ceremonies. Thunderdome reduces the overhead of running these sessions by providing a real-time, structured environment for:
- **Estimation alignment** — BAs can upload story backlogs (CSV/XML) and run estimation sessions without switching tools
- **Acceptance criteria capture** — Each story supports a rich-text description field and a dedicated Acceptance Criteria section (with Gherkin support)
- **Retrospective facilitation** — BAs can run structured retros and capture action items immediately
- **Story mapping workshops** — Map user journeys and feature hierarchies collaboratively with remote stakeholders
- **Async standups** — Maintain team visibility on blockers and progress without scheduling extra meetings

## How to use it in BA Workflows

### Planning Poker (Estimation)
1. Create a new **Battle** (planning session) and invite the team via link
2. Import stories from a CSV or XML export (e.g., from Jira) or add them manually
3. Add Acceptance Criteria per story using Gherkin (`Given / When / Then`) in the built-in editor
4. Run the vote — each participant picks a point value; results reveal only after everyone votes (prevents anchoring bias)
5. Discuss disagreements and re-vote until consensus is reached

### Sprint Retrospective
1. Create a **Retro** session and select a format (e.g., Start/Stop/Continue, 4Ls, Mad-Sad-Glad)
2. Participants add anonymous items; grouping and voting surfaces the most impactful themes
3. Export action items as a structured list for follow-up

### User Story Mapping
1. Create a **Storyboard** with goals (rows) and columns representing release phases
2. Add story cards under each goal/phase combination
3. Use the board to communicate scope and prioritization to stakeholders

### Async Standup
1. Configure a team standup with daily prompts (What did you do? What will you do? Blockers?)
2. Team members submit async updates — BA reviews blockers proactively before daily sync

## Key Features
- Real-time collaborative planning poker with simultaneous vote reveal
- Rich-text story editor with Acceptance Criteria (Gherkin-compatible)
- Story import/export via CSV and XML (Jira-compatible)
- Multiple retrospective formats built-in
- User story mapping board with goals, columns, and story cards
- Async team standup module
- Self-hostable via Docker + Postgres (full data ownership)
- Free hosted tier at [thunderdome.dev](https://thunderdome.dev)
- Open source under Apache 2.0 license

## GitHub Resources
- [StevenWeathers/thunderdome-planning-poker](https://github.com/StevenWeathers/thunderdome-planning-poker) — Main repository with source, Docker setup, and docs

## Related Skills
- [[Featmap - User Story Mapping]]
- [[Stakeholder Analysis Framework]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
- [[TextUSM - Text-Based Diagram Generator]]
