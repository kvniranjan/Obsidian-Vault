---
date: 2026-03-22
type: skill
category: Business Analysis
tags: [business-analyst, skill, automation, n8n, ai, workflow, reporting]
source: GitHub
---

# Automated Business Analysis Workflow (n8n + AI)

## What is it?
An open-source n8n workflow that scrapes any URL, uses AI models (Google Gemini + Perplexity) to analyze the content, and automatically generates a comprehensive business analysis report — delivered as a Google Doc, PDF, and email. Built for agencies, freelancers, and consultants who need rapid business intelligence.

GitHub: [AgriciDaniel/automated-business-analysis-workflow](https://github.com/AgriciDaniel/automated-business-analysis-workflow)

## Why it matters for Business Analysts
BAs frequently need to produce business overviews, stakeholder personas, and competitive analyses — often under time pressure. This workflow automates the most time-consuming parts of that research cycle: data gathering, synthesis, and document creation. Instead of spending hours manually compiling a business profile, a BA can generate a structured first-draft report in minutes and focus energy on validation and refinement.

It also demonstrates a practical pattern for AI-augmented BA work: trigger → scrape → AI analysis → structured output → delivery.

## How to use it in BA Workflows

### Setup
1. Import the `.json` workflow file into your n8n instance (self-hosted or cloud).
2. Connect Google Docs, Google Drive, Gmail, Perplexity, and Gemini credentials.
3. Configure your report template in Google Docs.

### Running an Analysis
1. Provide a target URL (client website, competitor, potential partner).
2. Trigger the workflow — n8n scrapes the page and passes content to AI agents.
3. Gemini + Perplexity extract structured intelligence and populate the report template.
4. The final PDF is saved to Drive and emailed to your inbox.

### BA Use Cases
- **Client onboarding:** Quickly generate a business overview before a discovery session.
- **Competitive analysis:** Run multiple competitor URLs and compare outputs.
- **Stakeholder prep:** Build persona profiles from prospect websites ahead of workshops.
- **Due diligence:** Rapid baseline analysis for new projects or vendors.

## Key Features
- Scrapes any public URL and extracts business-relevant content
- AI-generated sections: Business Overview, Target Audience Personas, Brand & UVP, Customer Journey Map, E-E-A-T Analysis
- Output formatted as a professional Google Doc from a reusable template
- Automatic PDF export + email delivery
- Pro version adds keyword research via DataForSEO (rankings, search volume, CPC, competitor data)
- Fully customizable — add or remove analysis sections by editing the workflow

## Technology Stack
| Component | Role |
|-----------|------|
| n8n | Workflow orchestration and automation engine |
| Google Gemini | AI analysis and structured extraction |
| Perplexity | Web-aware AI for enriched research |
| Google Docs/Drive | Report generation and storage |
| Gmail | Report delivery |

## GitHub Resources
- [AgriciDaniel/automated-business-analysis-workflow](https://github.com/AgriciDaniel/automated-business-analysis-workflow) — Main workflow repo with n8n JSON and setup instructions
- [n8n-io/n8n](https://github.com/n8n-io/n8n) — The underlying workflow automation platform (400+ integrations, self-hostable)

## Related Skills
- [[Stakeholder Analysis Framework]]
- [[BPMN Assistant (LLM-Powered)]]
- [[Featmap - User Story Mapping]]
