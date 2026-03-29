---
date: 2026-02-10
project: PI Planning and Operations
tags:
  - meeting
  - pi-planning
  - automation
  - archival
  - operations
---
# Runbook Automation and Archival Strategy for PI 19

**Date:** 2026-02-10
**Project:** [[PI Planning and Operations]]

## Database Security Issue
- Execute privileges incorrectly granted to read-only schema during package release
- Process improvement needed: strengthen code review, consider double-check peer review in JIRA

## UTI Automation User Clearing
- Only clear users if UTI fails due to user logged in
- Rare invocation (last used 2022)
- Testing planned: keep user logged in during batch run

## Action Items Review — Multiple CRs
- 4799956: Avinash follow-up pending
- 483644: Not approved, requires Flexibus review with J. Ganesh
- 494679: Approved after updates
- 505985: Description updated, Danny's review pending

## Archival and Purging Initiative
- Two epics created by Dawn for PI19 (499670 and 49961 for Brazil)
- Analysis phase only for PI19, implementation in PI20
- Current table list copied from Argentina — may not apply to Brazil
- Need CDP team input on applicable tables

## Runbook Automation Status
- Two items: few staging and trigger deferred deployment
- Flexibus staging already analyzed (two options: UDeploy or Rod)

## User Role Automation Challenges
- Certificate issues in dev environment (different approach than Canada)
- XSD differences between Canada and Brazil: two additional fields identified
- Friday deadline for UAT promotion

## Action Items
- [ ] Harry: Take archival analysis epic for PI19
- [ ] Amit: Runbook automation analysis (due this week)
- [ ] Email confirmation needed from PS on UTI automation scope
- [ ] Friday deadline for user role automation resolution
