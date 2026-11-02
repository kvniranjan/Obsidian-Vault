---
date: 2026-11-02
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, rules-engine, low-code, real-time-data, automation]
source: GitHub
---

# Nussknacker - Low-Code Real-Time Decision Engine

## What is it?
**Nussknacker** is an open-source, low-code visual tool for building, running, and monitoring real-time decision logic — created by TouK, a Polish software house. Instead of requiring IT to hard-code business logic, Nussknacker lets non-programmers (analysts, business people, domain experts) define decision algorithms in a step-by-step, readable visual form and deploy them directly into production streaming pipelines (built on Apache Flink or a lightweight Kubernetes-based engine), with syntax checking, autocompletion, versioning, debugging, and testing built into the Designer.

## Why it matters for Business Analysts
Many of the decisions a BA documents in requirements — "if transaction risk score exceeds X, flag for review," "if customer tier is gold and order value is above Y, apply discount Z" — end up buried in code that only developers can see or change, creating a translation gap and slow iteration cycles. Nussknacker closes that gap by giving BAs a no-code/low-code visual canvas to author, test, and own these decision rules end-to-end, without a developer handoff for every tweak. Because it operates on real-time streaming data (via Kafka/Flink), it's especially valuable for BAs working on fraud detection, credit/loan decisioning, next-best-offer, and real-time alerting use cases where logic changes need to ship fast and be auditable.

## How to use it in BA Workflows
1. **Fraud/risk rule authoring** - Model "is this transaction fraudulent?" logic as a visual scenario with conditional branches on transaction attributes, and deploy changes without waiting on a dev sprint.
2. **Loan/credit decisioning** - Define eligibility and approval logic (credit score thresholds, income bands, risk tiers) as readable decision scenarios that mirror how BAs already document approval criteria in BRDs.
3. **Next-best-offer and personalization rules** - Build real-time segmentation and offer-routing logic that reacts to live customer events, letting BAs iterate on targeting criteria directly.
4. **Testing and validation** - Use the Designer's built-in test panel to run sample data through a scenario before deployment, verifying the decision logic matches stakeholder-approved requirements.
5. **Change governance and monitoring** - Leverage built-in scenario versioning and monitoring to track who changed what rule and when, and observe live metrics on how rules are performing in production — supporting audit and compliance needs.

## Key Features
- Visual, low-code Designer for authoring decision scenarios without writing code
- Syntax checking, code completion, versioning, and debugging built into the editor
- Supports both streaming (Kafka/Flink) and request-response processing modes
- Lightweight Kubernetes-based engine option alongside full Flink deployment
- Built-in testing tools to validate scenarios against sample data before go-live
- Scenario versioning and monitoring for governance and production observability
- Designed explicitly so non-technical business users can own decision logic end-to-end

## Technology Stack
- **Languages:** Scala (core engine), with React-based frontend Designer
- **Dependencies:** Apache Flink (streaming engine), Kafka (primary streaming interface), optional Kubernetes-based lightweight engine
- **License:** Apache-2.0

## GitHub Resources
- [TouK/nussknacker](https://github.com/TouK/nussknacker) - Low-code tool for automating real-time decision logic, aimed at business analysts and domain experts

## Related Skills
- [[GoRules Zen - Open-Source Business Rules Engine]]
- [[Easy Rules - Lightweight Java Business Rules Engine]]
- [[Drools - Apache KIE Rule and DMN Decision Engine]]
- [[OpenL Tablets - Excel-Driven Business Rules Management System]]
- [[dmnmd - DMN Decision Tables in Markdown]]
