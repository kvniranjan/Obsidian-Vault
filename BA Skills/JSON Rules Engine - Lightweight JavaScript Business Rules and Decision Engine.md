---
date: 2026-10-07
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, business-rules, workflow-automation, data-analysis]
source: GitHub
---

# JSON Rules Engine - Lightweight JavaScript Business Rules and Decision Engine

## What is it?
json-rules-engine is a lightweight, isomorphic (Node.js and browser) rules engine that expresses business logic as plain JSON rule objects instead of hard-coded conditionals. Rules are composed of conditions (facts combined with ALL/ANY boolean operators, including recursive nesting) and events that fire when those conditions are met. It is secure by design (no `eval()`), fast, and ships with built-in TypeScript types.

## Why it matters for Business Analysts
Because rules live as structured JSON rather than buried in application code, a BA can read, review, and even draft decision logic directly - closing the gap between a documented business rule and its executable form. This makes it a practical reference implementation for decision management: it shows how eligibility criteria, approval thresholds, routing logic, or pricing rules can be externalized, versioned, and changed without a code deployment. For BAs working alongside engineering teams on decision tables, policy rules, or conditional workflow logic, it's a concrete, lightweight pattern to point to instead of a heavyweight BRMS.

## How to use it in BA Workflows
1. **Externalizing eligibility and approval rules** - Model documented business rules (e.g., "flag claims over $10,000 submitted by new customers for manual review") as JSON conditions and events, making the logic auditable by non-developers.
2. **Decision table prototyping** - Rapidly prototype decision logic gathered during requirements workshops before committing to a full DMN/BRMS platform, validating the rule set with stakeholders using readable JSON.
3. **Workflow routing and triage** - Drive conditional routing in automation pipelines (e.g., ticket escalation, approval chains) where facts about an entity determine the next workflow step.
4. **Requirements traceability for business logic** - Pair each JSON rule with its source requirement or policy document so changes to regulations or policy can be traced directly to the corresponding rule update.
5. **Data-driven validation rules** - Use the Almanac's fact caching to express validation or scoring logic against structured data sets, useful when BAs collaborate with data teams on data quality or segmentation rules.

## Key Features
- JSON-based rule definitions - conditions and events expressed as plain, version-controllable JSON instead of code.
- ALL/ANY boolean operators with recursive nesting for complex multi-condition logic.
- Almanac fact caching - computed facts are cached and reused across conditions within an engine run for performance.
- Secure by design - no `eval()`, reducing injection risk when rules come from external or user-editable sources.
- Isomorphic - runs identically in Node.js and the browser, and is lightweight (~17kb gzipped).

## Technology Stack
- **Languages:** JavaScript (with built-in TypeScript type declarations)
- **Dependencies:** clone, eventemitter2, hash-it, jsonpath-plus
- **License:** ISC

## GitHub Resources
- [CacheControl/json-rules-engine](https://github.com/CacheControl/json-rules-engine) - Lightweight, isomorphic JSON-based rules/decision engine for Node.js and the browser.

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
