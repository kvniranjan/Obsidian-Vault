---
date: 2026-07-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, use-case, ai-assisted, claude-ai, requirements, specification, iiba, karl-wiegers]
source: GitHub
---

# Use Case Writer - AI-Powered Use Case Specification Tool for Business Analysts

## What is it?
Use Case Writer is a Claude AI Skill designed for Business Analysts and Product Owners that scopes, analyzes, and documents Use Case Specifications in English Markdown. It strictly follows the 13-field Karl Wiegers / IIBA template, the industry-standard format for professional use case documentation. The skill runs natively inside Claude Code or claude.ai and acts as a structured AI mentor enforcing specification quality from the first draft.

## Why it matters for Business Analysts
Use cases are a foundational BA deliverable, yet junior analysts frequently struggle with completeness, precision, and consistent formatting across a project. This skill embeds the IIBA-endorsed 13-field structure into every generation, eliminating guesswork about what fields to include and how to phrase preconditions, postconditions, and alternate flows. It dramatically shortens the learning curve for new BAs — replacing months of trial-and-error with structured, mentor-quality output on day one. For experienced BAs it accelerates throughput by auto-drafting the boilerplate so analysts can focus on business logic validation and stakeholder review.

## How to use it in BA Workflows
1. **Drafting Use Case Specs from scratch** - Provide the skill with a feature name or user goal and it generates a complete 13-field use case document covering actors, preconditions, basic and alternate flows, postconditions, and business rules — ready for stakeholder review.
2. **Reviewing and enriching existing specs** - Paste an incomplete use case draft into Claude and activate the skill to identify missing fields, ambiguous steps, or gaps in alternate flows, then receive an enriched version with recommended improvements.
3. **Standardising cross-team documentation** - Embed the skill at the project level so all team members (BAs, POs, developers) generate use case artefacts in a consistent format, reducing review overhead and improving traceability.
4. **Onboarding junior Business Analysts** - Use the skill as a teaching tool: trainees submit their own draft, the AI highlights deviations from the Wiegers template, and annotates why each field matters — accelerating skills development.
5. **Feeding downstream artefacts** - Once a structured use case is generated, reference it as the source of truth for test case creation, user story decomposition, and acceptance criteria writing, maintaining tight requirements traceability.

## Key Features
- Follows the 13-field Karl Wiegers / IIBA Use Case Specification template for professional-grade output
- Generates Markdown-formatted documents compatible with Obsidian, Confluence, and documentation repos
- Four installation modes: user-level (~/.claude/skills/), project-level, claude.ai web, and one-shot prompt
- Acts as an AI mentor by enforcing standards and explaining deviations rather than silently fixing them
- Applicable to both waterfall use-case-driven projects and hybrid agile teams needing formal specification artefacts

## Technology Stack
- **Languages:** Markdown (output), natural language prompt engineering
- **Dependencies:** Claude AI (claude.ai or Claude Code CLI)
- **License:** Not specified (check repository)

## GitHub Resources
- [phucnt-bazone-vietnam/use-case-writer](https://github.com/phucnt-bazone-vietnam/use-case-writer) - Claude AI skill that scopes, analyzes, and documents Use Case Specifications following the 13-field Karl Wiegers / IIBA template

## Related Skills
- [[RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[OSRMT - Open Source Requirements Management Tool]]
