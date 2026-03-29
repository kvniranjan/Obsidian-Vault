---
date: 2026-02-12
project: ECS Plus Partner Integration
tags:
  - meeting
  - jtf
  - ecs-plus
  - onboarding
  - user-roles
---
# JTF Onboarding Configuration and User Role Mapping

**Date:** 2026-02-12
**Project:** [[ECS Plus Partner Integration]]

## JTF Onboarding Configuration
- Using XPI (175806) as base reference instead of XPY
- Key modifications required:
  1. Update dupe check constraints
  2. Change response stage from validation to "P" (after hitting daily log)
  3. Set response mode to non-EMS
  4. Remove CB reporting columns (not 24% partner)
- Offset posting remains "N" — file-based partner won't send offset entries

## Release Schedule Update
- April release cancelled (consent order only, same approach as February)
- Decision communicated by Tarun

## User Role Mapping Clarification
- Canada vs Brazil schema comparison revealed two unclear nodes (Role one, Master role description)
- Both fields are UI-only derivations — no external system mapping required
- Role information not in current CMP scope; future user role entitlement CMP planned separately

## Technical Issues
- MS code issue identified as CPV problem (mapping skipped during rollback changes)
- MCAR notification branch code fix: new column added to IFTB table with virtual branch logic

## Action Items
- [ ] Niranjan: Update dev task with JTF onboarding configuration details
- [ ] Team: Verify MCAR notification changes in UAT
- [ ] Outstanding: GBS/GPS project status unclear — no recent updates since Sep/Oct
