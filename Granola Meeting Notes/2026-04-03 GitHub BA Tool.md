---
date: 2026-04-03
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-04-03

## Repository
- **Name:** Freeplane
- **GitHub URL:** https://github.com/freeplane/freeplane
- **Stars:** ⭐ 4,000+
- **License:** GPL v2+
- **Last Updated:** 2026-03 (v1.13.2)

## What It Does
Freeplane is a mature, open source mind mapping and knowledge management application that runs on any platform with Java installed. It allows users to create rich, interactive mind maps — hierarchical diagrams of connected ideas — with support for notes, links, tasks, attributes, and formulas attached to each node. Beyond simple brainstorming, Freeplane is designed to function as a full knowledge management and lightweight project management tool, making it far more powerful than a typical mind map editor.

For a Business Analyst, Freeplane bridges the gap between freeform brainstorming and structured documentation. A BA can use it to facilitate stakeholder workshops, decompose complex problem domains, map out process flows at a conceptual level, structure interview questions, and organize knowledge gathered across multiple discovery sessions. Maps can be exported to HTML, PDF, Markdown, PNG, and other formats, and can be version-controlled in git alongside other project artifacts.

## Key Features
- Hierarchical mind maps with unlimited nesting depth, supporting both top-down and free-form layouts
- Rich node content: inline notes, hyperlinks, LaTeX formulas, embedded images, and file attachments
- Node attributes and filtering: add key-value metadata to nodes and filter/search across the entire map
- Built-in task management with task status, priority, and date attributes on individual nodes
- Scripting with Groovy for automating map transformations, report generation, and custom exports
- Multiple export formats: HTML, PDF, Markdown, SVG, PNG, OPML, and FreeMind-compatible XML
- Presentation mode ("Slideshow") that turns mind map branches into sequential slide presentations

## Installation
```bash
# Option 1: Download the installer for macOS/Windows/Linux from GitHub releases
# https://github.com/freeplane/freeplane/releases/latest

# Option 2: Homebrew (macOS)
brew install --cask freeplane

# Option 3: Portable ZIP (no install required, runs from USB)
# Download freeplane-<version>.zip, unzip, and run freeplane.sh (Linux/Mac) or freeplane.exe (Windows)

# Optional: Install Groovy for scripting automation
brew install groovy   # macOS
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Stakeholder Interview Preparation & Facilitation
Before a discovery interview or requirements workshop, create a Freeplane mind map with the central node named after the session (e.g., "Customer Portal Discovery — Sprint 1"). Add first-level branches for each topic area: "Current Pain Points", "Desired Outcomes", "Constraints", "Success Criteria", "Open Questions". Under each branch, pre-populate known sub-topics and talking points gathered from prior documentation. During the interview, navigate the map live as the conversation flows — adding new sub-nodes for each insight in real time. After the session, export the map to Markdown and paste it directly into your Obsidian meeting note under a `## Discovery Map` section. This gives you a structured, navigable record of everything discussed, far richer than bullet-point meeting minutes.

### 2. Problem Domain Decomposition for BRD Writing
When starting a Business Requirements Document, open Freeplane and create a central node for the initiative (e.g., "Loan Origination Modernisation"). Decompose it into branches: "Business Drivers", "In Scope", "Out of Scope", "Affected Stakeholders", "Key Processes", "Data Domains", "Assumptions & Constraints". For each branch, add child nodes capturing the actual requirements content. This visual decomposition lets you spot gaps — a branch with few children signals under-explored territory. Once the structure is stable, use Freeplane's export to generate an outline-structured Markdown file, which you then paste into Obsidian as the skeleton of your BRD: `[[BRD — Loan Origination Modernisation]]`. The mind map becomes both a thinking tool and a drafting accelerator.

### 3. Process Scope Mapping for BPMN Workshop Prep
Before running a BPMN process modelling workshop, use Freeplane to build a "process inventory" map: the central node is the process area (e.g., "Order Fulfilment"), first-level branches are sub-processes (Intake, Validation, Picking, Shipping, Returns), and second-level nodes are the specific activities, decision points, and handoff events within each sub-process. Color-code branches by department or system owner using Freeplane's node styles. Export the map as a PNG and embed it in your Obsidian pre-read note: `[[Workshop Pre-Read — Order Fulfilment BPMN]]`. Hand the PNG to workshop participants so everyone arrives with the same mental model of scope, dramatically reducing the "scope debate" time at the start of the session.

### 4. Knowledge Base for Running Projects
Create a persistent Freeplane map per project (e.g., `CRM-Replacement-Knowledge.mm`) stored inside your Obsidian vault. Use it as a living project knowledge base: one branch for key decisions (with date attributes), one for open issues, one for stakeholder contacts and their concerns, one for glossary terms, and one for links to key documents (requirements, minutes, diagrams). Add the Freeplane `.mm` file to your Obsidian vault and link to it from your project index note: `[Project Knowledge Map](CRM-Replacement-Knowledge.mm)`. Freeplane's node attributes allow you to tag nodes with status labels (`OPEN`, `DECIDED`, `DEFERRED`) and filter to show only open decisions at the start of each status meeting — giving you an instant "open items" agenda.

### 5. Slideshow Presentations for Stakeholder Reviews
Freeplane's built-in Presentation mode lets you convert any mind map into a sequential slideshow by marking which nodes should appear as slides. For a sprint review or steering committee update, structure a map with a branch per agenda item — "Progress Summary", "Decisions Required", "Risks", "Next Steps" — and mark each as a slide. Add detailed speaker notes to each node. During the meeting, run the Freeplane slideshow directly from the application rather than switching to PowerPoint. After the meeting, export the map as HTML and save it to Obsidian: `Stakeholder Reviews/2026-04-03 Steering Committee.html`. This eliminates the time spent reformatting PowerPoint decks between meetings while keeping a versioned record of every presentation in your vault.

## Why This Tool Today
Freeplane fills a gap that none of the previously discovered tools address: visual, free-form thinking and knowledge organisation at the conceptual level. While Doorstop and Specifai manage structured requirements in a repository, and Metabase handles data querying, a BA also needs a fluid thinking tool to work through ambiguous problem spaces before requirements are formalised. Freeplane's combination of mind mapping, task tracking, scripting, and presentation mode makes it a uniquely versatile companion for the full BA lifecycle — from the first blank-page discovery session through to stakeholder presentations. With 4,000+ GitHub stars and an active release in March 2026, it is one of the most mature and reliable open source tools in this space.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
