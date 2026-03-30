---
date: 2026-03-30
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-30

## Repository
- **Name:** Metabase
- **GitHub URL:** https://github.com/metabase/metabase
- **Stars:** ⭐ 46,700+
- **License:** AGPL v3 (Open Source Edition)
- **Last Updated:** 2026-03 (v0.60.0)

## What It Does
Metabase is an open source business intelligence and data analytics platform designed for everyone — not just engineers. It lets business analysts and non-technical stakeholders ask questions of their data through a visual query builder, receive auto-generated chart suggestions, and build interactive dashboards — all without writing a single line of SQL.

Metabase connects directly to databases (PostgreSQL, MySQL, BigQuery, Redshift, MongoDB, and 20+ more) and presents data exploration through a simple "notebook" interface where users filter, group, summarize, and visualize rows using dropdown menus. The result is that a BA can answer ad-hoc data questions in minutes rather than waiting on a data engineering queue, while also building persistent reports and dashboards for recurring stakeholder needs.

## Key Features
- Visual query builder ("Ask a Question") with filters, groupings, and aggregations — no SQL required
- Auto-generated visualizations: bar charts, line charts, pivot tables, maps, funnels, and more
- Interactive dashboards with drill-through filters, click behaviors, and auto-refresh
- SQL editor with autocomplete for power users who want to write their own queries
- Metabot AI assistant that generates queries from natural language prompts
- Scheduled reports delivered by email or Slack on a configurable cadence
- Public sharing links and embedded dashboards for stakeholder self-service

## Installation
```bash
# Option 1: Docker (fastest way to get started)
docker pull metabase/metabase
docker run -d -p 3000:3000 --name metabase metabase/metabase

# Option 2: Java JAR (requires Java 11+)
curl -O https://downloads.metabase.com/v0.60.0/metabase.jar
java -jar metabase.jar

# Open the web UI at http://localhost:3000 and run the setup wizard
# Connect your database (PostgreSQL, MySQL, BigQuery, etc.) in the wizard
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Self-Service Ad-Hoc Data Questions During Requirements Gathering
When working with a client to define requirements, BAs often need quick data snapshots: "How many users completed onboarding in the last 30 days?" or "What is the average ticket resolution time by product category?" With Metabase connected to your project's database, you can answer these in the visual query builder in under five minutes. In Obsidian, create a `Data Insights/` folder and paste the Metabase public link (using "Share → Public link") into your meeting notes. For example, in `Sprint 12 Requirements.md` add `- [Onboarding Completion Rate (live)](https://metabase.yourdomain.com/public/question/abc123)` so stakeholders always see live numbers, not a stale screenshot from last week.

### 2. Build a Stakeholder KPI Dashboard Before Every Status Review
Create a Metabase dashboard with the four or five metrics your project sponsor cares about most — delivery velocity, defect rate, user adoption rate, etc. Share the dashboard URL and embed it in your Obsidian weekly report template: `[[Templates/Weekly Status Report]]`. Before each status meeting, open the dashboard, apply the date filter for the current sprint, and screenshot the results for the slide deck. Because the queries are saved and reusable, you never spend time reformatting Excel charts — just refresh and present.

### 3. Replace Manual Excel Reports with Scheduled Deliveries
Metabase's "Subscriptions" feature lets you schedule any question or dashboard to be emailed to stakeholders as a PDF or inline HTML on a daily, weekly, or monthly cadence. Set up a "Monday Morning Business Report" that automatically emails the project sponsor every Monday at 8 AM with key metrics from the past week. In Obsidian, document the subscription setup in `Reporting/Automated Reports.md`, noting each subscription name, recipient, schedule, and what business question it answers. This frees you from manually pulling and distributing reports.

### 4. Data Profiling for UAT and Acceptance Criteria Validation
During UAT, BAs need to verify that data in the system matches acceptance criteria — e.g., "all orders placed after the cutover date must have the new product category codes." Use Metabase's SQL editor to write validation queries and save them as "Questions" in a collection named "UAT Validation — Sprint 14". Share the collection with the QA team. In Obsidian, link to each saved Metabase question from your UAT test cases: `| TC-042 | Verify category codes post-cutover | [Metabase Query](https://metabase.yourdomain.com/question/88) | Pass |`. This creates a traceable, data-backed UAT record that auditors can verify independently.

### 5. Exploratory Data Analysis to Inform Business Rules
Before writing functional requirements, a BA should understand the data landscape — outlier values, null rates, distribution of key fields — to write realistic and testable business rules. In Metabase, use the "X-ray" feature (click any table or column and select "X-ray this") to auto-generate a full statistical profile: row counts, cardinality, value distributions, and trend lines. Export the X-ray report as a PDF and attach it to your Obsidian requirements note: `[[BRD-007 Customer Segmentation Rules]]` with a section `## Data Profile` that embeds the findings. This grounds your business rules in actual data rather than assumptions.

## Why This Tool Today
Metabase fills a critical gap for BAs that none of the previously discovered tools address: self-service access to live operational data without engineering involvement. While ydata-profiling covers Python-based data profiling for data scientists, Metabase is built for non-technical users who need to query business databases through a web UI — the exact scenario a BA faces daily when needing quick data evidence to support decisions, validate requirements, or report to stakeholders. With 46,700+ GitHub stars and active development through 2026, it is one of the most mature and production-ready open source BI tools available.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
