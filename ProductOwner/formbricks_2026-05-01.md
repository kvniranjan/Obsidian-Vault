---
title: formbricks
date: 2026-05-01
tags:
  - product-owner
  - product-management
  - github
source: https://github.com/formbricks/formbricks
repo: formbricks/formbricks
status: recommended
---

# formbricks

## Verdict
This is genuinely worth a product owner's time if discovery, feedback collection, or product experiments are part of the job. Formbricks is not a PM reading list: it is a working survey and experience-management platform that can collect in-app, website, link, and email feedback. The blunt caveat is that a PO will still need engineering or ops help for serious self-hosting and product instrumentation.

## Repository
- Repository: [formbricks/formbricks](https://github.com/formbricks/formbricks)
- Owner/repo: `formbricks/formbricks`
- Primary language: TypeScript
- License: AGPLv3 for the core application, with separate enterprise-licensed code under `/apps/web/modules/ee`
- Stars: 12.2k
- Forks: 2.2k
- Open issues: 192
- Created date: 2022-06-06
- Last pushed date: GitHub organization listing showed updated 2026-04-19; latest visible release was 4.9.5 on 2026-04-29
- Main topics: `react`, `open-source`, `typescript`, `forms`, `reactjs`, `nextjs`, `form`, `survey`, `survey-data`, `typeform`, `surveys`, `survey-analysis`, `xm`, `survey-form`, `tailwindcss`, `turborepo`, `experience-management`

## Why This Repo Was Picked
It won because it directly supports product discovery and validation, which are daily PO problems when the team needs evidence instead of louder opinions. The repo has a mature product surface, survey templates, targeting, shareable link surveys, collaboration, integrations, hosted and self-hosted paths, active releases, and enough community usage to avoid looking like a weekend toy. It is more actionable than another product-management resource list and more broadly useful than a roadmap-only feedback board.

## Shortlist Considered
| Repo | What it offers | Why it did not win or why it won |
|---|---|---|
| [formbricks/formbricks](https://github.com/formbricks/formbricks) | Open-source survey and experience-management platform for in-app, web, link, and email feedback | Won because it helps a PO run discovery, validate assumptions, collect feedback, and analyze responses with less custom work |
| [QuackbackIO/quackback](https://github.com/QuackbackIO/quackback) | Open-source feedback board, public roadmap, changelog, integrations, and AI triage | Strong candidate, but younger and less proven; better for feedback loop operations than broad discovery |
| [logchimp/logchimp](https://github.com/logchimp/logchimp) | Self-hosted customer feedback, boards, roadmaps, and dashboard | Useful, but narrower than Formbricks and carries similar setup burden |
| [rowyio/roadmap](https://github.com/rowyio/roadmap) | Public roadmap voting app backed by Rowy and Firebase | Practical for roadmap voting, but too dependent on a specific backend path and less useful for discovery research |
| [opf/openproject](https://github.com/opf/openproject) | Full project management suite with roadmaps, work packages, agile boards, meetings, and planning | Mature, but too broad and operationally heavy for a PO looking for focused product-work leverage |

## What It Is
Formbricks is a software tool, not a template repo or framework document. The repository contains an open-source survey and experience-management application built with TypeScript, Next.js, React, Tailwind CSS, Prisma, Auth.js, Zod, and Vitest. It includes the web app, docs, Docker setup, OpenAPI definition, packages, deployment assets, and contribution material.

## Why It Is Useful For Product Owners
- Discovery: launch targeted surveys to validate customer problems before writing a bloated requirement.
- Backlog refinement: convert repeated survey feedback into clearer epics, user stories, and acceptance criteria.
- Prioritization: use response volume and segmentation as evidence when ranking roadmap candidates.
- Experimentation: run quick concept, pricing, onboarding, or feature-fit surveys before spending engineering time.
- Stakeholder alignment: bring actual customer responses into roadmap and scope debates instead of relying on internal opinions.
- Metrics: track NPS, satisfaction, product experience signals, and qualitative feedback around releases.
- Delivery coordination: use post-release surveys to check whether shipped work solved the intended problem.

## How I Would Actually Use It
1. Create a link survey for a risky roadmap item and send it to customers before committing it to the next quarter.
2. Add an in-app micro-survey after a key workflow to learn where users get stuck.
3. Run an NPS or CSAT survey after a major release and compare comments against the original success metrics.
4. Use templates to draft a product-market-fit, onboarding, cancellation, or feature-demand survey instead of starting from a blank form.
5. Pipe survey responses into Slack, Notion, Zapier, or n8n so feedback lands where the team already plans work.
6. Review survey analytics during backlog refinement and turn repeated pain points into story candidates with evidence attached.
7. Use self-hosting only when privacy, procurement, or data residency makes the hosted cloud path unacceptable.

## Limitations / Watch Outs
- Self-hosting is not a casual PO task. Docker helps, but production ownership still needs engineering or ops.
- The AGPLv3 core and enterprise-code split need legal review before company-wide adoption or modification.
- Survey tooling can produce fake confidence if questions are leading or the sample is biased.
- It does not replace interviews, usability testing, analytics, or customer calls. It complements them.
- Enterprise functionality may require a license key, so do not assume every README feature is free in every deployment mode.
- If the organization already has Qualtrics, Pendo, Sprig, UserVoice, or Productboard fully embedded, the switching cost may outweigh the benefit.

## Best Starting Points
- [README](https://github.com/formbricks/formbricks/blob/main/README.md)
- [Repository root](https://github.com/formbricks/formbricks)
- [Releases](https://github.com/formbricks/formbricks/releases)
- [Docs folder](https://github.com/formbricks/formbricks/tree/main/docs)
- [OpenAPI definition](https://github.com/formbricks/formbricks/blob/main/openapi.yml)
- [Docker assets](https://github.com/formbricks/formbricks/tree/main/docker)
- [Packages folder](https://github.com/formbricks/formbricks/tree/main/packages)
- [Self-hosting docs](https://formbricks.com/docs/self-hosting)

## Metadata
- Scan date: 2026-05-01
- Canonical repository URL: https://github.com/formbricks/formbricks
- Duplicate detection uses the canonical GitHub repository URL.
