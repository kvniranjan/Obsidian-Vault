---
date: 2026-03-10
project: ECS Plus Partner Integration
tags:
  - meeting
  - eflow
  - uat
  - account-creation
  - ecs-plus
---
# Account Creation Configuration for eflow UAT

**Date:** 2026-03-10
**Project:** [[ECS Plus Partner Integration]]

## Account Creation Configuration

- Current uncertainty about account class restrictions
  - Previously limited to specific account classes (from City Docs era)
  - Unclear if bypass implemented to allow all account classes
  - Need verification before eflow integration

## Eflow Integration Readiness

- ESCRE account class not yet available in eflow UAT — still in configuration phase
- Risk: account creation requests may fail at our end
- Need to prevent "account class not allowed" errors

## Project Timeline Status

- Q5 delivery target: May 2026
  - 99% confidence in May timeline
  - Potential spillover risk exists
- Outstanding dependencies:
  - PAT integration not sorted
  - Downstream systems not configured

## Configuration Updates

- CSI of ECS+ changed to new identifier
- UDF updates completed accordingly
- Ram confirmed changes implemented
