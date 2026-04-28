---
date: 2026-04-28
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, DMN, business-rules, rule-engine, decision-table, process-automation, java]
source: GitHub
---

# Drools - Apache KIE Rule and DMN Decision Engine

## What is it?
Drools is an open-source business rule management system (BRMS), DMN engine, and complex event processing (CEP) engine for Java and the JVM platform. Originally developed by Red Hat, it entered the Apache Software Foundation Incubator in 2023 as part of the Apache KIE project. It provides full conformance-level-3 support for the OMG DMN (Decision Model and Notation) standard, meaning every feature of the standard is supported at runtime.

## Why it matters for Business Analysts
BAs are increasingly expected to own and model business decisions, not just document them. Drools lets BAs define decision logic in DMN Decision Tables — a format understandable by non-developers — and execute those rules without hand-off to engineering. Its static analysis engine automatically detects gaps and overlaps in decision tables, catching logic errors before they reach production. The Decision Requirement Graph (DRG) provides a structured way to decompose complex decision hierarchies, making large-scale decision architecture visible and manageable. Because Drools integrates with BPMN process engines (like Camunda and jBPM), BAs can embed validated decisions directly into automated workflows.

## How to use it in BA Workflows
1. **Decision Table Authoring** - Design DMN decision tables in spreadsheet or visual form to express business rules (eligibility criteria, pricing tiers, approval logic) in a notation that business stakeholders can read and validate without developer involvement.
2. **Decision Requirement Graph (DRG) Design** - Decompose complex business decisions into sub-decisions using DRGs to clarify dependencies, trace decision lineage, and manage decision architecture across an enterprise.
3. **Automated Gap and Overlap Analysis** - Run Drools' built-in static analysis on decision tables to detect missing rule conditions (gaps) or conflicting rules (overlaps), reducing the risk of flawed decision logic reaching production.
4. **Requirements Validation via Executable Rules** - Convert textual business rules from requirements documents into executable Drools DRL or DMN models to validate that the implemented logic matches the stated requirement — providing a living test of requirements correctness.
5. **Complex Event Processing for BA Monitoring** - Use Drools' CEP engine to define event-driven business rules that monitor process streams in real time, enabling BAs to specify alerting and escalation logic for operational thresholds.

## Key Features
- **Full DMN 1.5 Conformance Level 3** — complete standard support for decision tables, decision services, and FEEL expression language
- **Decision Table Static Analysis** — automatic detection of gaps and overlaps in rule logic
- **DRL Rule Language** — expressive domain-specific language for complex forward/backward-chaining inference rules
- **Complex Event Processing (CEP)** — temporal and event-stream-based rule evaluation
- **BPMN/Process Integration** — pairs with jBPM, Camunda, and Flowable for embedding decisions in workflows
- **Kogito / Quarkus Support** — cloud-native deployment of decision services as microservices
- **PMML Integration** — import predictive models (ML) alongside business rules in a unified engine

## Technology Stack
- **Languages:** Java (primary), FEEL (DMN expression language), DRL (Drools Rule Language)
- **Dependencies:** Maven, JVM 11+, Quarkus (optional cloud-native runtime)
- **License:** Apache License 2.0

## GitHub Resources
- [apache/incubator-kie-drools](https://github.com/apache/incubator-kie-drools) - Rule engine, DMN engine and CEP engine for Java; 6,200+ stars

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
