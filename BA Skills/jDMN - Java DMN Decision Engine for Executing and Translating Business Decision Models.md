---
date: 2026-08-04
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, dmn, decision-model, business-rules, java, decision-table, decision-automation]
source: GitHub
---

# jDMN - Java DMN Decision Engine for Executing and Translating Business Decision Models

## What is it?
jDMN is a Java implementation of the OMG Decision Model and Notation (DMN) standard, created and open-sourced by Goldman Sachs. It provides both an interpreter for running DMN decisions at runtime and a translator that converts DMN decision tables into type-safe Java code for deployment in enterprise systems. The library supports the full DMN specification including decision tables, boxed expressions, and FEEL (Friendly Enough Expression Language).

## Why it matters for Business Analysts
Decision Model and Notation (DMN) is the standard language BAs use to document and communicate business decision logic — the rules that determine outcomes like loan eligibility, pricing tiers, or compliance classifications. jDMN bridges the critical gap between a BA's decision model and its technical implementation: rather than handing a DMN file to developers and hoping for a faithful translation, jDMN executes the BA's model directly or generates Java code that mirrors it exactly. This reduces specification drift and lets BAs validate decision logic before it goes into production. The Goldman Sachs provenance signals that the library is proven in high-stakes, high-volume financial decision environments, making it trustworthy for enterprise BA workflows.

## How to use it in BA Workflows
1. **Decision Table Validation** - Model decision tables in a DMN-compliant tool (Camunda Modeler, dmn-js), then run jDMN's interpreter against sample inputs to verify outputs before sign-off, catching logic errors at the requirements stage rather than in UAT.
2. **Requirements-to-Code Traceability** - Use jDMN's code generation to produce Java implementations that are named and structured identically to the BA's decision model, making traceability between business requirements and code explicit and auditable.
3. **Automated Acceptance Testing** - Generate decision test cases in the DMN test annotation format and run them via jDMN to create a living test suite tied directly to the business requirements document, which re-runs on every code change.
4. **Collaborative Rule Discovery Workshops** - Share DMN XML files with stakeholders after facilitation sessions; use jDMN to demo live execution of the agreed rules on real data, providing immediate confirmation that the model captures the intended business logic.
5. **Regulatory and Audit Documentation** - Export executable DMN models alongside jDMN-generated test reports as evidence that implemented decision logic precisely matches the documented business rules — valuable for compliance reviews and audit trails in regulated industries.

## Key Features
- **Full DMN Interpreter** - Executes `.dmn` files at runtime without compilation, enabling rapid iteration during BA workshops
- **DMN-to-Java Translator** - Generates strongly-typed Java classes from DMN models, preserving decision names and structure for traceability
- **FEEL Language Support** - Full support for DMN's Friendly Enough Expression Language, which is designed to be readable by business stakeholders
- **Decision Table Hit Policies** - Supports all DMN hit policies (UNIQUE, FIRST, PRIORITY, ANY, COLLECT, RULE ORDER, OUTPUT ORDER) that BAs use to express conflict resolution logic
- **Test Case Generation** - Can generate and execute DMN decision test cases to verify model correctness
- **Multi-language Runtimes** - Companion repositories provide Python (`jdmn-python-runtime`) and JavaScript (`jdmn-js-runtime`) runtimes for translated decisions
- **Enterprise Pedigree** - Developed by Goldman Sachs and actively maintained; used in production financial systems since 2018

## Technology Stack
- **Languages:** Java (core), with Python and JavaScript runtime companions
- **Dependencies:** Maven; Java 11+; Apache Commons, Jackson
- **DMN Standard:** OMG DMN 1.2 / 1.3
- **License:** Apache License 2.0

## GitHub Resources
- [goldmansachs/jdmn](https://github.com/goldmansachs/jdmn) - Java DMN interpreter and code generator by Goldman Sachs

## Related Skills
- [[dmn-js - Browser-Based DMN Decision Table Viewer and Editor]]
- [[dmnmd - DMN Decision Tables in Markdown]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[Fluxnova - FINOS Open-Source BPMN and DMN Process Orchestration Platform]]
- [[Camunda - BPMN Process Orchestration Framework]]
