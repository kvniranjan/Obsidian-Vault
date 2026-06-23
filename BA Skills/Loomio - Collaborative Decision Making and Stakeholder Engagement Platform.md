---
date: 2026-06-23
type: skill
category: Business Analysis
tags: [business-analyst, skill, decision-management, stakeholder-analysis, collaboration, requirements, consensus-building, open-source]
source: GitHub
---

# Loomio - Collaborative Decision Making and Stakeholder Engagement Platform

## What is it?
Loomio is an open-source web application that helps groups make better decisions together through structured discussion, formal proposals, and consent-based voting. Built on Ruby on Rails, it provides a permanent, auditable record of discussions and decisions across distributed teams. It is deployed in over 100 countries and supports 35 languages, making it suitable for large, geographically dispersed stakeholder groups.

## Why it matters for Business Analysts
BAs frequently face the challenge of driving consensus among diverse stakeholders with competing priorities — Loomio provides a structured platform for that process rather than relying on informal emails or meeting notes. Its formal proposal workflow forces stakeholders to articulate their position explicitly (agree, abstain, disagree, block), producing clear signal on where alignment exists and where it doesn't. The permanent decision archive gives BAs an auditable trail linking requirements decisions back to stakeholder input, which is invaluable for change management and traceability. The threaded discussion model keeps context attached to each decision, reducing the context loss that plagues requirements elicitation done over email chains.

## How to use it in BA Workflows
1. **Requirements Sign-Off** - Create a formal Loomio proposal for each requirement baseline, invite stakeholders to vote agree/disagree/abstain, and close the proposal once quorum is reached — producing a dated, attributable approval record.
2. **Prioritization Voting** - Use Loomio polls (ranked choice, dot voting, or score voting) to facilitate backlog prioritization sessions asynchronously, eliminating the need for every stakeholder to attend a live meeting.
3. **Stakeholder Consensus on Scope Changes** - When change requests arrive, post the change rationale as a Loomio thread, collect structured reactions, and use the proposal outcome to document the formal decision rather than relying on verbal agreement.
4. **Workshop Follow-Up** - After requirements workshops, post key decisions and open questions to Loomio threads so remote or absent stakeholders can contribute, and the discussion becomes part of the project record.
5. **Risk and Assumption Validation** - Surface identified risks or assumptions as Loomio proposals and ask stakeholders to vote on their validity, capturing dissenting views that might otherwise surface only in post-launch retrospectives.

## Key Features
- **Formal proposals** with configurable voting methods: consent, simple majority, ranked choice, time-boxed polls
- **Threaded discussions** that keep context and rationale attached to every decision
- **Decision archive** providing a searchable, permanent audit trail of all outcomes
- **Subgroups** for organizing stakeholders by domain, team, or project phase
- **@mentions and subscriptions** ensuring the right people are notified without inbox flooding
- **Self-hostable** via Docker (loomio/loomio-deploy) for organizations with data residency requirements
- **API access** enabling integration with project management and requirements tools

## Technology Stack
- **Languages:** Ruby (Rails), JavaScript (Vue.js)
- **Dependencies:** PostgreSQL, Redis, Docker
- **License:** GNU Affero General Public License v3.0 (AGPL-3.0)

## GitHub Resources
- [loomio/loomio](https://github.com/loomio/loomio) - Open-source collaborative decision-making platform with 2.5k stars

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[Thunderdome - Agile Planning and Retro Suite]]
- [[MetaGPT - Multi-Agent Requirements and Document Generation Framework]]
- [[GoRules Zen - Open-Source Business Rules Engine]]
