---
date: 2026-05-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, kanban, backlog-management, ai-assisted, git, user-stories, agile, task-management]
source: GitHub
---

# Backlog.md - AI-Native Kanban and Task Management for Git

## What is it?
Backlog.md is an open-source, Markdown-native task manager and Kanban visualizer built for Git repositories. It stores every task as a plain `.md` file, making your backlog human-readable, version-controlled, and directly accessible to AI coding assistants. It runs entirely offline with zero configuration, and is installable via npm, bun, or brew.

## Why it matters for Business Analysts
BAs often struggle to keep requirements and task backlogs synchronized with developer workflows and AI tools. Backlog.md bridges that gap by storing tasks as structured Markdown files inside the repository itself, ensuring requirements, acceptance criteria, and user stories live alongside the code they describe. It natively integrates with AI agents like Claude Code, Gemini CLI, and MCP-compatible assistants, enabling AI to read, create, and update tasks in a format already familiar to BAs. Because the backlog is Git-native, BAs gain full version history, branching, and audit trails on every requirement change — capabilities typically reserved for heavyweight enterprise tools.

## How to use it in BA Workflows
1. **Requirements Capture** - Create tasks directly from discovery sessions using `backlog task create "As a user, I want to..."`, populating acceptance criteria, priority, and labels in a plain Markdown file that the whole team can review and edit.
2. **Kanban Visualization** - Run `backlog board` to instantly render an interactive terminal Kanban board, or use the web interface to give non-technical stakeholders a visual sprint view without requiring any project management SaaS subscription.
3. **AI-Assisted Backlog Refinement** - Point Claude Code or another MCP-compatible AI at the backlog folder; the AI can read task descriptions, suggest missing acceptance criteria, identify duplicate requirements, or draft new tasks from meeting notes automatically.
4. **Traceability and Audit** - Because all tasks are Git-tracked Markdown files, BAs can use `git log` or `git blame` on any task to see who changed acceptance criteria, when, and why — satisfying traceability requirements for regulated industries.
5. **Sprint Planning and Filtering** - Use `backlog task list --filter status=todo label=sprint-3` to slice the backlog by sprint, label, or assignee, then export the board view for stakeholder review or handoff documentation.

## Key Features
- **Markdown-native tasks** - Each task is a `.md` file with YAML frontmatter for status, priority, and labels; editable in any text editor
- **AI-ready CLI** - Provides structured plain-text outputs and an `AGENTS.md` instruction file so AI agents can reliably interact with the backlog
- **Zero-configuration** - No database, no server, no cloud dependency; works fully offline from day one
- **Terminal Kanban board** - Instant visual board via `backlog board` for sprint or backlog overviews in the terminal
- **Web UI** - Modern browser-based interface for visual task management and board export for stakeholder sharing
- **Rich query commands** - Filter and search tasks by status, label, assignee, or free text across all task files
- **MCP connector support** - Compatible with Model Context Protocol, enabling deep integration with Claude Code and other AI development environments
- **Cross-platform** - Runs on macOS, Linux, and Windows

## Technology Stack
- **Languages:** TypeScript
- **Runtime/Bundler:** Bun
- **CLI Framework:** Commander.js
- **Dependencies:** Zero external runtime dependencies; distributed as an npm package
- **License:** MIT

## GitHub Resources
- [MrLesk/Backlog.md](https://github.com/MrLesk/Backlog.md) - Markdown-native task manager and Kanban visualizer for human-AI collaboration in Git repositories

## Related Skills
- [[Featmap - User Story Mapping]]
- [[rmToo - Git-Native Requirements Management Tool]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[LangGraph - AI Agent Orchestration Framework]]
- [[n8n - Fair-Code Workflow Automation Platform]]
