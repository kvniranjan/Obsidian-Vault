---
date: 2026-02-13
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - flexcube
  - posting
  - earmarking
  - kafka
---
# FlexCube Consolidated Posting and Earmarking Workflow

**Date:** 2026-02-13
**Project:** [[FlexCube Brazil Payments]]

## Consolidated Posting Implementation
- No additional changes needed beyond existing XPI/XPY source code creation
- ICD updates include new T-codes with incoming/outgoing mappings
- Consolidated posting for both incoming and outgoing payments (previously only itemized)
- Same consolidated approach used globally

## Date Handling & Transaction Processing
- Transaction initiation date always sent as current calendar date
- Business date and TRN date functionally identical in FlexCube
- Boundary condition: transactions after midnight categorized as next day
  - Ledger posting happens on next business day
  - Available balance updated immediately but tanked until EOD

## Brazil-Specific Requirements
- Book-to-book transfers will use 4-leg posting structure (debit/credit nostro and debit/credit account)
- Similar to Australia model to avoid clearing charges
- Kafka topic structure: consolidated posting uses separate topic (global standard)
- Account scope: ~8,000 accounts (vs 4,000 in Argentina)

## Outgoing Payment Flow & Earmarking
- New earmarking request required before posting
- Earmark reference number included in posting requests
- Transaction type clarification needed: FU (force update) vs PR (posting request) against earmarks
- Pre-green zone earmarking challenges:
  - 30-minute monthly green zone window
  - Cannot send earmark requests for all 8,000 accounts
  - Need account list for pre-green zone eligibility

## Action Items
- [ ] Ravi/Deepak: Confirm TLM field layout sharing
- [ ] Team: Review ICD when circulated
- [ ] Niranjan: Check PR vs FU transaction type requirements internally
- [ ] Product team (Christina/Jennifer/Monica): Prioritize capacity increase (200 TPS) discussion
- [ ] Ricardo: Provide account list for pre-green zone earmarking eligibility
