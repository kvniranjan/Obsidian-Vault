---
date: 2026-02-06
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - flexcube
  - earmarking
  - gccs
  - c-core
---
# Investigating Earmark and Transaction Flow GCCS vs C Core

**Date:** 2026-02-06
**Project:** [[FlexCube Brazil Payments]]

## Earmarking Flow Investigation
- Investigating earmarking flow for bank transactions
- Received earmark request from GCCS as of December 30th
- EB (earmarking within balance) showing correct amount block number
- CATM amount blocks showing zero amount despite active earmark

## Current System Architecture Issues
- C Core only sending memo transactions
- GCCS handling earmarks separately
- Flow doesn't align with expected BAU operations
  - C Core should provide transactions against earmarks
  - Current separation creates operational gaps
- Online transactions via Zebra vs batch feed processing

## Transaction Flow Analysis
- Memo against earmark showing as debit transaction
- Amount matching but transaction type questionable
- No memo flag found at transactional level
- Successfully processed transactions without proper memo classification

## Proposed Flow
1. Bank contacts GCCS for earmark reference number
2. Bank sends confirmed transaction against earmark
3. Eliminates memo-first approach
- Memo deletion will release earmark and reinstate block
- Confirmed transaction posts against reinstated block

## Action Items
- [ ] CC: Analyze Zebra table for additional verification
- [ ] Revise mechanism between GCCS and C Core
