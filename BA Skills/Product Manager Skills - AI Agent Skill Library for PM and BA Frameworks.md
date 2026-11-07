---
date: 2026-11-07
type: skill
category: Business Analysis
tags: [business-analyst, skill, ai-assisted-workflows, requirements, stakeholder-analysis, prioritization]
source: GitHub
---

# Product Manager Skills - AI Agent Skill Library for PM and BA Frameworks

## What is it?
Product Manager Skills is an open-source library of 77 structured `SKILL.md` files, each encoding a battle-tested product management framework (its purpose, key concepts, application steps, examples, and common pitfalls) in a format AI agents can read and apply directly. It is designed to plug into Claude Code, Claude Desktop/Web, Codex, ChatGPT, Cursor, and other agents that read structured markdown, as well as to teach the underlying reasoning to a human practitioner.

## Why it matters for Business Analysts
Many of the included frameworks map directly onto core BA deliverables: writing PRDs, user stories, and epics; running stakeholder alignment and discovery sessions; prioritizing and roadmapping scope; and performing market/competitive intelligence. Because each skill is a self-contained, reusable prompt artifact rather than a one-off ChatGPT conversation, a BA can invoke the same vetted reasoning repeatedly across projects, keeping output consistent and reducing generic, unreliable AI output. The library also includes an "AI product work" category, useful for BAs gathering requirements for AI-enabled features. It's a practical reference implementation of how to package domain expertise as reusable AI skills - a pattern directly transferable to building a BA-specific skill set.

## How to use it in BA Workflows
1. **Requirements and deliverable drafting** - Use the "Writing PM deliverables" skills (PRDs, user stories, epics) as templates an agent can fill in from stakeholder notes, keeping structure and terminology consistent across a backlog.
2. **Stakeholder alignment** - Apply the stakeholder alignment skills to structure RACI-style mapping, influence/interest analysis, and communication plans before kicking off requirements workshops.
3. **Discovery and research** - Run the customer discovery and research skills to turn raw interview notes or survey data into structured insights that feed a requirements document.
4. **Prioritization and roadmapping** - Use the prioritization/roadmapping skills (e.g., scoring frameworks) to turn a raw backlog into a justified, stakeholder-ready roadmap.
5. **Interactive elicitation** - Leverage the "Interactive skills" tier, which asks 3-5 guided questions before producing numbered recommendations, as a lightweight way to run structured elicitation sessions with an AI agent standing in for a facilitator.

## Key Features
- **Three skill tiers** - Workflow skills (end-to-end processes), Interactive skills (guided Q&A then recommendations), and Component skills (deliverable templates), covering different levels of engagement.
- **Consistent SKILL.md structure** - Frontmatter, Purpose, Input, Key Concepts, Application, Examples, Common Pitfalls, and References, making skills predictable to read and extend.
- **Multi-platform compatibility** - Works with Claude Code, Claude Desktop/Web, Codex, ChatGPT, Cursor, and any agent that reads structured markdown, not locked to one vendor.
- **Streamlit playground (beta)** - A browsable, no-install web app with "Learn," "Find My Skill," and "Run Skills" modes for non-developers, supporting Anthropic, OpenAI, and Ollama providers.
- **Guided start routes** - Entry points tailored to a situation (an unvalidated idea, a new mandate, an aging product) rather than a flat skill list.

## Technology Stack
- **Languages:** Markdown (skill definitions, templates, documentation); Python (Streamlit playground app)
- **Dependencies:** Streamlit, with multi-provider LLM support for Anthropic, OpenAI, and Ollama via API keys; packaged as ZIP skill packs and a Claude Code plugin marketplace entry
- **License:** CC BY-NC-SA 4.0 (non-commercial use and share-alike adaptation with attribution; reselling the skills themselves is not permitted)

## GitHub Resources
- [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) - Open-source library of 77 AI-agent-readable product management skill frameworks.

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts]]
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Storymaps.io - Real-Time Collaborative User Story Mapping Tool]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
