---
date: 2026-07-16
type: skill
category: Business Analysis
tags: [business-analyst, skill, requirements-management, ai-assisted, user-stories, requirements-quality, incose, llm]
source: GitHub
---

# RequirementLinter - AI-Powered User Story and Requirements Quality Reviewer

## What is it?
RequirementLinter is an open-source, AI-powered tool that reviews user stories and requirements against established industry guidelines, specifically the International Council of Systems Engineering (INCOSE) Guide to Writing Requirements (GtWR). It uses an LLM to analyse each requirement, identify weaknesses, and suggest concrete improvements to make them clearer, more measurable, and correctly structured. The tool also includes a lightweight pre-check that uses a smaller model to determine whether the input even resembles a valid requirement before running the full analysis.

## Why it matters for Business Analysts
Business Analysts frequently write requirements and user stories that are technically valid but fail quality checks — they are ambiguous, untestable, or incomplete. RequirementLinter automates the peer-review step by applying the INCOSE GtWR standard consistently, catching issues that manual review often misses. This raises the bar for requirements quality before they reach development teams, reducing costly rework caused by misunderstood or under-specified stories. For BAs working in agile or regulated environments, having a standards-aligned linting step embedded in the workflow provides audit-ready evidence of requirements rigour and helps junior analysts learn the craft faster through AI-generated feedback.

## How to use it in BA Workflows
1. **Pre-sprint requirements review** - Run user stories through RequirementLinter before sprint planning to surface ambiguous acceptance criteria, missing measurability, or structural issues, ensuring stories are ready for estimation.
2. **Backlog grooming quality gate** - Integrate the linter as a step in your backlog refinement process so every story receives INCOSE-aligned feedback before it progresses from "Draft" to "Ready", maintaining consistent quality across a large backlog.
3. **Junior BA coaching** - Use the tool's suggested improvements as learning material for junior analysts, providing concrete before-and-after examples that illustrate what good requirements look like according to international standards.
4. **Regulatory compliance documentation** - In regulated industries (finance, healthcare, aerospace), run the linter over requirements artefacts to generate evidence that requirements meet a recognised writing standard, supporting audit and traceability obligations.
5. **Iterative requirements refinement** - Feed the linter's suggestions back into the requirement, re-run until the score improves, and track the evolution of requirements quality over time as a measurable BA team metric.

## Key Features
- **INCOSE GtWR alignment** — Validates requirements against the industry-standard Guide to Writing Requirements for consistent, professional quality
- **LLM-powered analysis** — Uses GPT-4-class models to understand context and suggest semantically meaningful improvements, not just syntax checks
- **Pre-check fast path** — A lightweight validity check using a smaller, faster model filters non-requirement inputs before the full analysis runs
- **Prompt-driven architecture** — Guidelines are loaded from markdown files, making the validation rules transparent and customisable for domain-specific standards
- **Structured improvement suggestions** — Returns a revised, improved version of the requirement alongside an explanation, making feedback actionable immediately

## Technology Stack
- **Languages:** TypeScript / Node.js
- **Dependencies:** OpenAI API (GPT-4), markdown-based prompt/guideline files
- **License:** MIT

## GitHub Resources
- [jonverrier/RequirementLinter](https://github.com/jonverrier/RequirementLinter) - AI-powered tool for reviewing and improving user stories and requirements against INCOSE GtWR guidelines

## Related Skills
- [[GitHub Spec-Kit - AI-Powered Spec-Driven Development Toolkit]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[Lore RAC-Core - Requirements as Code for AI-Assisted BA Workflows]]
- [[OpenFastTrace - Requirements Traceability Suite]]
- [[OSRMT - Open Source Requirements Management Tool]]
