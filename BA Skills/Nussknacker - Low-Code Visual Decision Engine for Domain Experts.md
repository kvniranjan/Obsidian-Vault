---
date: 2026-09-29
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, low-code, workflow-automation, rules-engine]
source: GitHub
---

# Nussknacker - Low-Code Visual Decision Engine for Domain Experts

## What is it?
Nussknacker is an open-source, low-code platform that lets non-technical domain experts build, test, and deploy real-time decision algorithms through a visual scenario editor instead of writing code. It processes streaming (Kafka-based) or request-response (HTTP/OpenAPI) data to make automated decisions such as fraud detection, offer routing, or alerting, using prebuilt components for filtering, aggregation, enrichment, and transformation.

## Why it matters for Business Analysts
Nussknacker is purpose-built to put decision logic authoring directly in the hands of analysts and subject-matter experts, closing the classic gap between "what the business wants" and "what gets implemented." Because scenarios are visual and testable in a sandbox, a BA can iterate on business rules (eligibility checks, routing logic, scoring thresholds) in minutes without waiting on a developer sprint. It pairs naturally with decision management and requirements work: the visual scenario becomes both the specification and the executable artifact, reducing translation loss between requirements documents and system behavior. It also gives BAs a concrete tool to reference when documenting decision tables, business rules, or event-driven process logic in BPMN/DMN-adjacent initiatives.

## How to use it in BA Workflows
1. **Decision logic specification as executable artifact** - Model business rules (e.g., discount eligibility, fraud flags, SLA routing) directly as a visual scenario, so the "requirement" and the "implementation" are the same reviewable diagram.
2. **Rapid rule prototyping and validation** - Use the built-in testing/sandbox environment to run sample data through a proposed rule set and validate outcomes with stakeholders before formal sign-off.
3. **Cross-functional collaboration** - Share the visual scenario editor with both business stakeholders and engineers as a single source of truth, cutting down ambiguity in handoff documents.
4. **Process monitoring and traceability** - Leverage integrated monitoring (event counts per step) to show stakeholders how a decision process behaves in production, supporting audits and continuous improvement.
5. **Integration mapping for requirements** - Use the component library (SQL, OpenAPI, ML model enrichment) to document what data sources and systems a decision process depends on, informing data and integration requirements.

## Key Features
- Visual scenario editor with syntax checking and code completion for building decision logic without traditional coding
- Multiple processing modes: streaming (Kafka), request-response (HTTP/OpenAPI), and batch (in development)
- Data enrichment via SQL, OpenAPI endpoints, and ML models for context-aware decisions
- Integrated monitoring and metrics tracking algorithm behavior step-by-step
- Sandbox testing/debugging so rule changes can be validated before deployment
- Horizontally scalable, Kubernetes-native architecture for enterprise deployment

## Technology Stack
- **Languages:** Scala (core engine), JavaScript/TypeScript (frontend), SpEL (expression language for rule logic)
- **Dependencies:** Apache Kafka, Apache Flink, Kubernetes, Docker/Helm
- **License:** Apache License 2.0

## GitHub Resources
- [TouK/nussknacker](https://github.com/TouK/nussknacker) - Low-code visual tool for domain experts to build and monitor real-time decision algorithms

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[jDMN - Java DMN Decision Engine for Executing and Translating Business Decision Models]]
