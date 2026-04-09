---
date: 2026-04-08
project: FlexCube Brazil Payments
tags:
  - meeting
  - ecs-plus
  - payment-to-cards
  - defect
  - uat
  - debit-posting
---
# Troubleshooting Payment to Cards Transaction

**Date:** 2026-04-08
**Project:** [[FlexCube Brazil Payments]]

## Payment Flow Issue

- ECS Plus unable to identify transactions due to incorrect additional text field
  - Expected: "payment to cards" identifier
  - Receiving: "wire payment real time manual" or other values
  - Root cause: Shanmukpriya triggered transactions without proper additional text
- Transaction status: failed at debit posting stage
  - Source identifier validation error preventing processing
  - No successful debit posting in DB tables yet
- Request ID from yesterday 9:45 AM IST needs history table lookup
  - Not indexed; will require time to search

## Additional Text Field Requirements

- All transactions (credit/debit) from ECS Plus must include "payment to cards"
- Field enables proper transaction identification and processing
- Credit vs debit flow distinction:
  - Automated credits from ECS Plus: always "payment to cards"
  - Manual credits via Flex UI: can have different values (acceptable)
  - External client credits: impact OTB limits and relationship balances

## Resolution Path

- Subu's mala issue fix promoted to UAT — debit posting can be re-triggered tomorrow
- Srini and Manju will provide support for re-triggering
- No immediate action required for existing credit notifications with different values
- Documentation needs updating in user story/DAG for additional text field requirements

## Action Items

- [ ] Shanmukpriya — Use "payment to cards" in additional text for future test transactions
- [ ] Srini / Manju — Support re-triggering debit posting after UAT promotion
- [ ] Niranjan — Update user story/DAG documentation for additional text field requirements
- [ ] Journey — Discuss credit notification testing requirements separately with team
