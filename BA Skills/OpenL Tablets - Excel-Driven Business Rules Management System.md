---
date: 2026-05-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, business-rules, decision-tables, excel, decision-management, no-code, brms]
source: GitHub
---

# OpenL Tablets - Excel-Driven Business Rules Management System

## What is it?
OpenL Tablets is an open-source Business Rules Management System (BRMS) that allows business analysts to define, test, and manage decision logic directly inside Microsoft Excel spreadsheets. The platform compiles those spreadsheets into high-performance Java bytecode and exposes the rules as production-ready REST APIs. It supports decision tables, decision trees, and decision graphs, and integrates with AI assistants (Claude, ChatGPT) via MCP protocol.

## Why it matters for Business Analysts
BAs are often the domain experts who understand the business rules, but must rely on developers to translate them into code — creating bottlenecks and introducing translation errors. OpenL Tablets closes that gap: BAs write rules in Excel using familiar syntax, test them with real data in a browser-based studio, and deploy changes without writing a single line of code. The compile-time validation catches conflicts and gaps before rules reach production, making governance much tighter. The AI/MCP integration also means BAs can query and update rule logic through conversational interfaces.

## How to use it in BA Workflows
1. **Decision Table Authoring** - Model complex branching logic (pricing, eligibility, classification) as structured Excel tables with conditions and actions — no programming required. OpenL validates the table for completeness and conflicts at save time.
2. **Business Rule Testing** - Use the built-in OpenL Studio web UI to run test cases against rule tables with real or synthetic data, catching regression errors before handoff to developers.
3. **Rule Versioning and Governance** - Store rule files in Git repositories; OpenL's Rules Repository tracks change history, enabling BAs to compare rule versions and roll back decisions independently.
4. **REST API Deployment** - Publish approved rule packages as OpenAPI-documented REST endpoints that downstream applications consume — BA-owned rules become live services without a dev sprint.
5. **AI-Assisted Rule Maintenance** - Connect Claude or ChatGPT via the MCP protocol to query existing rule tables in plain language, identify gaps, or draft new rule rows, accelerating analysis of large or complex rule sets.

## Key Features
- **No-code Excel authoring** - Decision tables, trees, and graphs written in standard `.xlsx` files
- **OpenL Studio** - Browser-based IDE for editing, testing, and publishing rule packages
- **Compile-time validation** - Detects unreachable rows, type mismatches, and logic gaps before deployment
- **REST API generation** - Automatic OpenAPI spec generation from rule packages
- **Git-backed repository** - Rule versioning and branching via standard Git workflows
- **AI/MCP integration** - First-class support for Claude and ChatGPT as rule authoring assistants
- **High performance** - Excel rules compile to native Java bytecode; capable of millions of decisions per second
- **LGPL license** - Can be embedded in commercial products with limited copyleft obligations

## Technology Stack
- **Languages:** Java (core engine), Excel/XLSX (rule authoring)
- **Dependencies:** Spring Boot, Jakarta EE 10 (OpenL Studio), Git (rules repository)
- **License:** GNU Lesser General Public License (LGPL)

## GitHub Resources
- [openl-tablets/openl-tablets](https://github.com/openl-tablets/openl-tablets) - OpenL Tablets Business Rules Management System

## Related Skills
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Camunda - BPMN Process Orchestration Framework]]
