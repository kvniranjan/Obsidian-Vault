---
date: 2026-04-08
project: FlexCube Brazil Payments
tags:
  - meeting
  - payment-hub
  - json
  - float-account
  - dag
  - pi19
---
# JSON Data Mapping for Payment Hub Integration

**Date:** 2026-04-08
**Project:** [[FlexCube Brazil Payments]]

## JSON Data Format Confirmation

- Final version confirmed for data exchange
- Same JSON structure for day zero and day one feeds
- Payment hub uses different file format but identical content
  - Enables shared storage approach for both systems

## Day Zero Data Source

- Baseline data available from payment hub before CPX integration goes live
- Trina previously confirmed this approach
- Need to verify current payment hub data extraction process
  - Unclear if already taking baseline from payment hub

## Float Account Mapping

- Row 15: Float account number
- Linked account: Quadum account field
- Float customer number matches linkage number
- All required data present for Codom resolution

## Timeline

- DAG approval needed before development pickup
- Target: Approval by end of this week
- Development scheduled for PI 19 (June release target)

## Action Items

- [ ] Niranjan — Check payment hub day zero feed extraction process
- [ ] Niranjan — Confirm June release timeline after DAG approval
