---
date: 2026-02-12
project: ECS Plus Partner Integration
tags:
  - meeting
  - brazil
  - ecs-plus
  - go-code
---
# Brazil Transaction Model and GO Code Setup with ECS Plus

**Date:** 2026-02-12
**Project:** [[ECS Plus Partner Integration]]

## Brazil Model Implementation
- No MIS code system in Brazil — direct GO code setup instead of 9,988 universal code
- GO code will be used for traffic routing
- SH team will use this code for notifications

## ECS Plus Integration
- ECS Plus won't interact directly with GO code
- Process flow:
  1. Cash account creation triggers mapping in processor
  2. SH team sends notifications based on GO code
  3. Real-time balance updates (increase/decrease) against company

## Process Changes Required
- Onboarding modifications: switch from 9,988 to GO code basis
- Update FlexCube maintenance location
- All notifications sent against new GO code (Brazil limitation prevents 9,988 maintenance)

## Action Items
- [ ] Niranjan: Email team confirming GO code usage instead of 9,988
- [ ] Niranjan: Inform ECS Plus team about notification changes via GO code
- [ ] Check with Nityan tomorrow about implementation
