---
date: 2026-03-26
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-modeling, DMN, requirements, rules, markdown]
source: GitHub
---

# dmnmd — Decision Model & Notation in Markdown

## What is it?
**dmnmd** is an open-source CLI tool that lets you write DMN (Decision Model & Notation) decision tables using plain Markdown table syntax, then parse, evaluate, and translate them into executable formats (JavaScript, and future targets including Python, XML, and LegalRuleML).

Rather than using heavyweight XML editors or proprietary GUI tools, dmnmd follows the Unix philosophy: keep business rules in flat, human-readable text files that live naturally in version control.

- GitHub: [smucclaw/dmnmd](https://github.com/smucclaw/dmnmd)
- Standard: Based on the OMG [DMN 1.3 standard](https://www.omg.org/dmn/)

## Why it matters for Business Analysts
BAs routinely capture business rules in decision tables — loan eligibility, pricing tiers, approval thresholds, policy exceptions. Traditionally these live in Excel, Confluence, or proprietary BPMN tools that are hard to version, diff, or automate.

dmnmd brings decision tables into the same plain-text, version-controlled world as code:
- Rules become reviewable in pull requests alongside the software they drive
- Non-technical stakeholders can read and edit Markdown tables
- Output can be directly consumed by developers as JavaScript logic
- Aligns with Agile/DevOps practices where docs-as-code is valued

## How to use it in BA Workflows

### 1. Author a decision table in Markdown
Write your business rule as a standard Markdown table. Example — loan approval by credit score and income:

```markdown
| Credit Score | Annual Income | Loan Decision |
|---|---|---|
| >= 750       | any           | Approved      |
| 650–749      | >= 50000      | Approved      |
| 650–749      | < 50000       | Review        |
| < 650        | any           | Declined      |
```

### 2. Run the dmnmd CLI to evaluate
Pass an input row to get a decision output:
```bash
dmnmd eval table.md --input "CreditScore=700, AnnualIncome=60000"
# Output: Approved
```

### 3. Export to JavaScript for developers
```bash
dmnmd translate table.md --output decisions.js
```

### 4. Embed in your requirements document
Because the tables are just Markdown, they can live inside your BRD, user story acceptance criteria, or wiki pages without any special tooling.

## Key Features
- Plain-text Markdown table syntax — no XML, no GUI required
- CLI interpreter for parsing, evaluating, and translating tables
- Version control-friendly: tables diff cleanly in git
- JavaScript output for direct developer handoff
- Based on the OMG DMN 1.3 standard — compatible with industry tooling
- Supports FEEL (Friendly Enough Expression Language) expressions in cells
- Designed for compliance/legal rule encoding as well as standard BA use cases

## GitHub Resources
- [smucclaw/dmnmd](https://github.com/smucclaw/dmnmd) — Main repo: CLI tool for DMN tables in Markdown
- [dmn-tck/tck](https://github.com/dmn-tck/tck) — DMN Technology Compatibility Kit for testing DMN engines
- [red6/dmn-check](https://github.com/red6/dmn-check) — Static analysis tool to detect bugs in DMN files
- [ungerts/awesome-bpm](https://github.com/ungerts/awesome-bpm) — Curated list of BPM/DMN tools and resources

## Related Skills
- [[bpmn-io Web Modeler]]
- [[BPMN Assistant (LLM-Powered)]]
- [[PM4Py - Process Mining for Business Analysts]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
