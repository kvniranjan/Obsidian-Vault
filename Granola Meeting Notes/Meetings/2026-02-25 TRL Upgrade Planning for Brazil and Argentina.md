---
date: 2026-02-25
project: TRL Upgrade
tags:
  - meeting
  - trl
  - brazil
  - argentina
  - costa-rica
  - regulatory
---
# TRL Upgrade Planning for Brazil and Argentina

**Date:** 2026-02-25
**Project:** [[TRL Upgrade]]

## TRL Upgrade Timeline
- No confirmed dates for Brazil/Argentina TRL upgrade deployment
- Current tentative plan:
  - Loans: August-September
  - Deposits: October-November
- Team prefers separate rollouts due to complexity
- Planning hampered by Genesis team's changing requirements

## Null Value Population Requirements
- Mandatory field for TRL20: accounts with maturity type "Evergreen"
- Will populate as exception for 2-3 months post go-live until TRL21
- Source feed implementation in TRL22
- Load-only testing being evaluated vs. full UAT

## Country-Specific Issues
- **Argentina (March 10th code drop confirmed):** 533 contracts with maturity date exceptions; overdraft agreements using fixed maturity (should be Evergreen); premature withdrawal indicator populated as "Y" for all products
- **Brazil (July target):** All accounts treated as loans; simpler implementation
- **Costa Rica:** June deployment confirmed for 1308 item

## Resource Allocation
- Pooja available for 15-day development window (50% allocation)
- CQE capacity constraints with multiple V4 items in parallel

## Action Items
- [ ] Niranjan: Raise SRT today for all three countries (Argentina maturity type corrections)
- [ ] Share SRT details with team
- [ ] Confirm resource availability with Ram for three-country deployment
