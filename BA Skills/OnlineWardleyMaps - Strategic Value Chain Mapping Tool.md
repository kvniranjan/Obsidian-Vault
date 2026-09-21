---
date: 2026-09-21
type: skill
category: Business Analysis
tags: [business-analyst, skill, wardley-mapping, strategy-mapping, capability-mapping, process-modeling, stakeholder-analysis]
source: GitHub
---

# OnlineWardleyMaps - Strategic Value Chain Mapping Tool

## What is it?
OnlineWardleyMaps is a free, open-source tool for creating Wardley Maps — a strategic visualization method developed by Simon Wardley that plots the components of a value chain against their evolutionary stage (from novel/genesis to commodity). It's available as a web app at onlinewardleymaps.com, a VS Code extension, and an Obsidian.md plugin, and stores maps as plain-text `.owm` files that can be version-controlled like code.

## Why it matters for Business Analysts
Wardley Mapping gives BAs a way to visualize the current-state business landscape — user needs, capabilities, and their supporting components — and reason about how each piece is evolving over time. This is invaluable for current-state/future-state analysis, prioritizing where to invest versus outsource or commoditize, and communicating strategic context to stakeholders in workshops. Because maps are plain text, they fit naturally into a BA's documentation-as-code toolkit alongside BPMN and DMN artifacts, and can be diffed and reviewed like any other requirements document.

## How to use it in BA Workflows
1. **Current-State Landscape Analysis** — Map the value chain from user need down through supporting capabilities and infrastructure to visualize dependencies before writing requirements.
2. **Build vs. Buy vs. Outsource Decisions** — Use the evolution axis (genesis → custom-built → product → commodity) to identify which components are strategic differentiators worth custom development versus commodity services worth outsourcing or buying off the shelf.
3. **Stakeholder Workshops** — Facilitate collaborative mapping sessions where stakeholders jointly place components on the map, surfacing disagreements about priorities and dependencies early.
4. **Roadmap and Investment Prioritization** — Overlay planned initiatives on the map to show how the organization intends to move components along the evolution axis, supporting business case narratives.
5. **Documentation-as-Code Integration** — Store `.owm` map files in the same git repository as BPMN diagrams and requirements specs, versioning strategic context alongside detailed process and requirements artifacts.

## Key Features
- Plain-text `.owm` map syntax that renders instantly in the browser, VS Code, or Obsidian
- Evolution axis (genesis, custom-built, product, commodity) plus value chain axis for two-dimensional strategic positioning
- Map annotations, pipelines, and evolution markers for showing planned change over time
- Local API and Docker/docker-compose support for self-hosted deployment
- VS Code and Obsidian.md extensions for editing maps alongside other documentation

## Technology Stack
- **Languages:** TypeScript, JavaScript (React/Node.js)
- **Dependencies:** Node.js, Yarn; Docker optional for self-hosted deployment
- **License:** MIT (map notation itself is CC BY-SA 4.0, per Simon Wardley)

## GitHub Resources
- [damonsk/onlinewardleymaps](https://github.com/damonsk/onlinewardleymaps) - Free online tool for creating Wardley Maps in seconds, with VS Code and Obsidian integrations

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[ContextMapper DSL - Domain-Driven Design Context Mapping and Service Decomposition]]
- [[PlantUML - Diagrams-as-Code for Business Analysts]]
