---
date: 2026-02-11
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - flexcube
  - sweeps
  - weekend-processing
---
# Brazil Flex Market Seven Day Sweeps Implementation

**Date:** 2026-02-11
**Project:** [[FlexCube Brazil Payments]]

## Transaction Processing Options Analysis

### Option 1: Seven-Day Processing (Recommended)
- Enable weekend balance file generation for Saturday/Sunday
- GC configures seven-day sweep capability (existing feature in US/Thailand markets)
- Requires EOD signals for holiday dates
- Minimal GC development effort — mostly configuration changes
- Flex changes: generate balance/transaction files for weekends + EOD trigger signals

### Option 2: Enhanced BBT File Grouping
- Add earmark amount and earmark value date fields to BBT file
- Group transactions by earmark value date
- Concerns: requires ICD changes and GC logic modifications

### Option 3: Earmark-Based Processing (Least Preferred)
- Extract transactions based on earmark creation date instead of transaction date
- Major challenges: earmarks have multiple statuses, complex history tracking

## Current Problem Context
- Earmark created Saturday, transaction posted Sunday
- Creates timing mismatches between earmark and transaction processing
- Volume constraints previously drove weekend processing, now resolved with netting logic

## Action Items
- [ ] Finalize option recommendations for management review (focus on Option 1)
- [ ] Amit: Check with dev team on Flex-side implementation requirements
- [ ] Arundan: Confirm GC configuration needs and testing scope
- [ ] Send analysis to Ajit today with recommended approach
