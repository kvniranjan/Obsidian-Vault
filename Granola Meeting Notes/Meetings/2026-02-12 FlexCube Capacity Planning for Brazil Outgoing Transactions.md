---
date: 2026-02-12
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - flexcube
  - capacity
  - performance
---
# FlexCube Capacity Planning for Brazil Outgoing Transactions

**Date:** 2026-02-12
**Project:** [[FlexCube Brazil Payments]]

## Capacity Requirements
- Current commitment: 200 TPS for P99 latency <2 seconds (combined earmarking + posting)
- Requested enhancement: separate capacity — 200 TPS earmarking + 200 TPS posting (total 400 TPS)
- Current production baseline: <100 TPS maximum observed
- Argentina comparison: 225 TPS (earmarking only)

## Advanced Earmarking Strategy
- Business push for day-one implementation on high-volume clients
  - Target clients: Uber, PayPal, Rappi (top 3 Brazil clients)
  - Advanced earmarking reduces frequency to once per 4 hours
  - Expected shift: mostly posting transactions vs earmarking

## Account Funding Scenarios
- Two-tier SLA structure needed:
  1. Sufficiently funded accounts: Target 200 TPS with <2 second latency
  2. Insufficient funds requiring C900 lookup: Degraded performance acceptable
- Brazil-specific: netting balance across customer portfolio accounts

## Integration Architecture Changes
- Current: GPP -> FlexCube integration
- Day one: GLS -> FlexCube integration (same C900 dependency)
- Future: GLS direct C900 integration (removes C900 dependency from FlexCube)

## Action Items
- [ ] Niranjan: Internal discussion on capacity scaling requirements
- [ ] Niranjan: Assess production trends for Uber, PayPal, Rappi netting structures
- [ ] Niranjan: Provide two-scenario SLA breakdown (funded vs unfunded)
- [ ] Pending: Liquidity Pod decision on GLS-C900 integration approach
