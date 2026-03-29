---
date: 2026-02-26
project: GL Reclassification
tags:
  - meeting
  - brazil
  - gl
  - accounting
  - reclassification
---
# Interim GL and Account Class Reclassification Strategy

**Date:** 2026-02-26
**Project:** [[GL Reclassification]]

## Technical Issue Overview
- Toxic combination at FFS side where loan asset reporting from DDA
- Interim GL approach proposed to resolve sync issues
  - Include credit account class for OED reclass
  - Lending side entry for ADB account (debit SHGL, credit interim GL)
  - Will sync up when goes to FFS

## Implementation Approach
- Using CL side reclassification for ADB side entry
- Key challenge: determining correct dimension for common balance
- Need to identify external JS samples for three entry sets:
  1. Interim debit term
  2. New interim GL (already created)
  3. Final credits (existing)

## Dimension Configuration Analysis
- CLPG has own defined dimensions
- Options: use existing dimension with process code modifications OR implement additional parameter
- Priority: rule out existing dimension usage before adding new parameters

## Account Setup & Balance Transfer
- New interim GL account (299) being introduced
- Standard script needed to move balances from current to new GL
- Brazil system differences: relies only on common balance (not GL system like Argentina/Canada)

## Action Items
- [ ] Check production balance for existing GL account
- [ ] Determine dimension requirements for new setup
- [ ] Confirm balance transfer approach with team
- [ ] Consider reverse reclassification impact on existing entries
- [ ] End-to-end testing required for all ADV scenarios
