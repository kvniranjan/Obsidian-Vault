---
date: 2026-04-03
type: skill
category: Business Analysis
tags: [business-analyst, skill, product-roadmap, stakeholder-management, feedback, requirements, prioritization]
source: GitHub
---

# Ploi Roadmap - Product Feedback and Roadmapping

## What is it?
Ploi Roadmap is a self-hostable, open source product roadmapping and customer feedback management tool built with Laravel (PHP). It provides a public-facing portal where stakeholders and users can submit feature requests, report bugs, and upvote existing items — giving BAs a structured, transparent channel to capture and prioritize the voice of the customer without relying on expensive SaaS tools like Canny or ProductBoard.

The platform supports a lightweight role system (administrator, employee, and user), configurable workflow states (e.g., Planned, In Progress, Shipped, Declined), and auto-generated slugs and Open Graph images so roadmap items are shareable with stakeholders in a single link.

A standout feature for technical BA teams is the GitHub integration, which links roadmap items directly to GitHub issues or milestones, creating a lightweight traceability chain from customer request to engineering delivery. An `/ai` endpoint also exposes each item as machine-readable JSON, making it easy to feed roadmap data into LLMs like Claude for automated reporting or backlog summaries.

## Why it matters for Business Analysts
BAs are often responsible for gathering, organizing, and communicating stakeholder needs — a process that typically lives in scattered emails, Jira comments, and ad hoc Slack threads. Ploi Roadmap centralizes this by providing:
- **Structured feedback capture** — Stakeholders submit requests through a consistent form rather than unstructured channels, making requirements easier to review and triage
- **Quantified prioritization** — Upvote counts give BAs an objective, data-backed signal of business value when ranking backlog items
- **Transparent stakeholder communication** — Status updates on roadmap items replace repetitive "what's the status?" emails with a self-serve, always-current view
- **Traceability** — GitHub integration links each business request to its engineering issue, supporting audit trails and impact analysis
- **AI-assisted reporting** — The `/ai` endpoint enables automated stakeholder updates and backlog analysis via LLM prompts

## How to use it in BA Workflows

### Setting Up a Feedback Portal
1. Deploy Ploi Roadmap via Docker or a standard Laravel host (see Installation below)
2. Configure item categories matching your domain (e.g., Features, Bugs, Improvements, Integrations)
3. Set up workflow statuses that reflect your delivery process (Backlog → Planned → In Progress → Shipped)
4. Share the public portal URL with internal stakeholders, pilot users, or product owners
5. Link the portal URL from your Obsidian project index note: `[Feedback Portal](https://roadmap.yourteam.com)`

### Prioritizing Backlog Items
1. Review the portal weekly and sort items by upvote count to surface high-demand requests
2. Export top-voted items and copy them into your Obsidian sprint planning note alongside effort estimates
3. Use upvote counts as a MoSCoW or WSJF input during backlog grooming sessions with the team
4. Update item statuses after each sprint so the roadmap reflects current delivery progress

### GitHub Traceability
1. Enable the GitHub integration by adding your `GITHUB_TOKEN` and `GITHUB_REPO` to the `.env` config
2. For each roadmap item that is accepted into development, link it to its GitHub issue from the admin panel
3. Reference the roadmap item URL in your Obsidian BRD or user story note to create a full trace: business need → roadmap item → GitHub issue → pull request

### AI-Assisted Stakeholder Reporting
1. Call the `/ai` endpoint for a roadmap item (e.g., `GET /roadmap-item-slug/ai`) to retrieve structured JSON
2. Paste the JSON into a Claude prompt: *"Summarize these roadmap items for a non-technical stakeholder update, grouped by status"*
3. Copy the generated summary into your Obsidian meeting note or weekly stakeholder email

## Key Features
- Public roadmap portal for submitting and upvoting feature requests and bug reports
- Upvoting system to quantify and surface highest-demand items
- Role-based access control (administrator, employee, user)
- Configurable item workflow statuses (Planned, In Progress, Shipped, Declined, etc.)
- GitHub integration to link roadmap items to issues and milestones
- AI-friendly `/ai` endpoint returning machine-readable JSON per roadmap item
- Auto-generated slugs and Open Graph images for shareable, professional links
- Self-hostable via Docker + MySQL/PostgreSQL (full data ownership)
- 554 stars on GitHub | MIT License | Actively maintained

## Installation
```bash
# Clone the repository
git clone https://github.com/ploi/roadmap.git
cd roadmap

# Install PHP and JS dependencies
composer install
npm install && npm run build

# Configure environment
cp .env.example .env
php artisan key:generate

# Run migrations and seed default data
php artisan migrate --seed

# Optional: Enable GitHub integration in .env
# GITHUB_TOKEN=your_personal_access_token
# GITHUB_REPO=org/repo-name

# Start the server
php artisan serve
```

## GitHub Resources
- [ploi/roadmap](https://github.com/ploi/roadmap) — Main repository with source, Docker setup, and changelog

## Related Skills
- [[Featmap - User Story Mapping]]
- [[Stakeholder Analysis Framework]]
- [[Thunderdome - Agile Planning and Retro Suite]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
