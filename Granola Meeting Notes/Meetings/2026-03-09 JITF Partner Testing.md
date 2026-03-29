---
date: 2026-03-09
project: JTF Onboarding
tags:
  - meeting
  - jitf
  - golden-gate
  - database
---
# ECS Plus Partner Integration

**Date:** 2026-03-09
**Project:** [[ECS Plus Partner Integration]]

## Database Configuration Discussion

- Golden Gate connectivity requires main DB access, not shadow DB
- Current setup uses shadow DB only for Golden Gate
- Key issue: MITB class mapping table (main driving table for filtration) doesn't replicate to shadow DB
  - Transaction details replicate successfully to shadow
  - MITB class mapping is critical for filtering operations
- DBA team initially provided shadow DB details assuming full replication

## Required Database Changes

- Need main DB connectivity for Golden Gate project
- Two tables require replication setup:
  1. MITB class mapping
  2. CSTB ADDL text
- Testing approach will be hybrid:
  - Part of testing on shadow DB
  - Part of testing on main DB
- Configuration change, not system change

## Project Setup Clarification

- Waiting on clarity about Iran's cash account setup
- New GLC involved but purpose unclear
- NFT and ELI components are part of overall project scope

## Action Items

- [ ] Forward main DB requirements to DBA group via existing email thread
- [ ] DBA team to provide main DB details for Golden Gate connectivity
- [ ] Follow up with Iran regarding cash account setup intentions
- [ ] Update progress in Teams channel
