---
date: 2026-02-13
project: TRL Upgrade
tags:
  - meeting
  - trl
  - loan-mapping
  - data-mapping
---
# Map Gap Document Review for Loan Product Mapping

**Date:** 2026-02-13
**Project:** [[TRL Upgrade]]

## Mapping Document Review
- Reviewed map gap document against existing logic for multiple fields
- Found several discrepancies between proposed and current mappings
- Interest payment frequency code mapping appears identical to existing logic — no changes needed

## Missing Conditions & Updates Required
- Look back days field missing rate variability type condition (need to add type 2)
- Contract rate currency code missing type 2 condition
- Daily floor cap per red flag also needs type 2 addition
- Multiple fields defaulting to null don't require condition checks

## Frequency Code Mapping Changes
- Bi-weekly mapping discrepancy identified — missing 1014 code
- Monthly: 1003 (correct), Bi-weekly: 1014 (needs addition), Semi-annually: 1005 (correct)

## Complex Logic Clarifications
- Multiple unit records handling: if account has both weekly and monthly units, default to 1008
- Contract spread rate percentage logic involves rate code conditions across effective dates
  - Prioritize rate code = null when both conditions exist

## Action Items
- [ ] Niranjan: Update mapping document with missing rate variability type 2 conditions
- [ ] Niranjan: Add bi-weekly frequency code (1014) to mapping
- [ ] Niranjan: Update document today, share updated version
- [ ] Puja: Verify record flow patterns for multiple unit handling
- [ ] Puja: Check contract spread rate derivation logic
