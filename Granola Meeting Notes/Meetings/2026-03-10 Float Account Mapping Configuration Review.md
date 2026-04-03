---
date: 2026-03-10
projects:
  - FlexCube Brazil Payments
  - Amcar Integration
tags:
  - meeting
  - float-account
  - mapping
  - configuration
---
# Float Account Mapping Configuration Review

**Date:** 2026-03-10
**Projects:** [[FlexCube Brazil Payments]], [[Amcar Integration]]

## Account Mapping Configuration

- Float account system uses one-to-one mapping structure
  - One Quadam account maps to exactly one Float account
  - Same Quadam account can map to multiple protocols
- Relationship management constraints
  - Cannot modify existing relationships directly
  - Must close current relationship before creating new record

## System Logging Behavior

- Notifications bypass standard notification log
  - Routes to separate table instead
  - Different tracking mechanism than expected

## Administrative Controls

- Account management capabilities
  - Can modify expiry dates on existing mappings
  - Can close mappings when needed
- Relationship closure process
  - Requires full closure of existing relationship
  - New record creation necessary for changes

## Technical Clarifications

- Confirmed Float/Jirada system integration
- Mapping limitations clearly defined
- One-to-many protocol support verified
