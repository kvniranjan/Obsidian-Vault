---
date: 2026-08-07
type: skill
category: Business Analysis
tags: [business-analyst, skill, trend-monitoring, social-listening, competitive-intelligence, ai-analysis, market-research, stakeholder-insights, mcp]
source: GitHub
---

# TrendRadar — AI-Driven Public Opinion and Trend Monitoring Platform

## What is it?
TrendRadar is an open-source, AI-driven trend monitoring and public opinion analysis tool that aggregates multi-platform hotspots with RSS support and smart alerts. It uses LLMs to filter news intelligently, translate content, and generate structured analysis briefs, with MCP architecture support for natural language querying of trends and sentiment insights. Deployable via Docker and GitHub Actions, it delivers alerts through Slack, Telegram, email, and other channels.

## Why it matters for Business Analysts
Business Analysts need current, synthesized intelligence about market trends, stakeholder sentiment, and competitive dynamics to inform requirements and strategic decisions. TrendRadar automates the laborious process of monitoring multiple information sources — news, social platforms, and RSS feeds — and applies AI analysis to surface what matters. Its MCP integration means BAs can query trend data conversationally through AI agents, accelerating the translation of market signals into business requirements. The multi-channel notification system ensures timely alerts about sentiment shifts or emerging topics relevant to a domain, without constant manual monitoring.

## How to use it in BA Workflows
1. **Competitive Intelligence Gathering** - Configure TrendRadar to monitor keywords related to competitors, products, and industry trends; receive daily AI-summarized briefs on competitive landscape changes to inform strategy sessions and business cases.
2. **Stakeholder Sentiment Monitoring** - Set up keyword tracking for product names, company mentions, and known customer pain points; use AI sentiment analysis to understand stakeholder perceptions before workshops or interviews.
3. **Requirements Discovery from Market Signals** - Monitor industry forums and news for emerging customer needs, regulatory changes, and technology shifts; translate trend alerts into candidate requirements or change requests for the backlog.
4. **Strategic Planning Intelligence** - Subscribe to sector-specific RSS feeds and configure weekly AI analysis briefs; use synthesized trend summaries to support roadmap decisions and priority arguments.
5. **MCP-Powered Natural Language Trend Queries** - Integrate TrendRadar with an MCP-compatible AI assistant to ask conversational questions such as "What are the top concerns about X in the last 30 days?" and receive structured trend analysis without manual report generation.

## Key Features
- **Multi-platform aggregation** — Monitors diverse sources including news platforms, social media, and custom RSS feeds simultaneously
- **AI news filtering** — LLM-powered relevance scoring removes noise, surfacing only meaningful signals from high-volume feeds
- **AI translation** — Automatically translates non-English content, enabling global market and competitor monitoring
- **AI analysis briefs** — Generates concise, structured summaries pushed directly to phone or email on schedule
- **MCP architecture support** — Enables natural language conversation, sentiment insights, and trend prediction via AI agents
- **Flexible notification channels** — Supports Slack, Telegram, email, ntfy, DingTalk, Feishu, WeChat, and Bark
- **Three push modes** — Daily summary, current rankings, and incremental (real-time) monitoring
- **Docker deployment** — Simple self-hosted setup with local or cloud data storage options
- **GitHub Actions integration** — Runs automated monitoring on a schedule without a dedicated server

## Technology Stack
- **Languages:** Python
- **Dependencies:** Docker, GitHub Actions, configurable LLM APIs (OpenAI-compatible)
- **License:** MIT

## GitHub Resources
- [sansan0/TrendRadar](https://github.com/sansan0/TrendRadar) — AI-driven public opinion and trend monitor with multi-platform aggregation, RSS, and smart alerts

## Related Skills
- [[Automated Business Analysis Workflow (n8n + AI)]]
- [[n8n - Fair-Code Workflow Automation Platform]]
- [[Dify - Production-Ready AI Agentic Workflow Platform]]
- [[PandasAI - Conversational AI Data Analysis for Business Analysts]]
- [[Evidence - SQL and Markdown Business Intelligence Reporting Platform]]
- [[RAGFlow - Deep Document Understanding and AI-Powered Knowledge Extraction]]
