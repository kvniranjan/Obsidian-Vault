---
date: 2026-03-20
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - earmarking
  - gls
  - express
---
# Clarifications on Earmarking and Release Request Process for GLS

**Date:** 2026-03-20
**Project:** [[FlexCube Brazil Payments]]

## Express Flow Implementation Status

- All queries answered by Trina's team regarding CPX RT requirements
- One pending item: need to send limit check as "EL" (Earmark within limits) to GLS
  - Currently not implemented or using default value
  - GLS needs this to pass through to downstream systems
- ICD documentation straightforward — same as GPP1 with no changes needed

## Brazil Earmark Process Changes

- No future-dated earmarks in new Express flow (contrary to user stories)
- New process: release requests sent same day instead of using expiry dates
  - Expiry date will be null
  - Closure request sent by end of day
- Current GPP flow: null expiry date with no closure request, amount stays blocked
- Express flow improvement: will receive closure requests same day

## Performance Impact Assessment

- Need to evaluate system performance with increased closure requests
- Estimated impact: if 10% of earmarks don't get corresponding transactions, need closure requests
- NFT testing must include this new flow
  - Approach: assume 100% closure requests (2x current volume for safety)
  - Need realistic count estimates from appropriate team members
- Most GPP requests follow earmark-first-then-debit pattern

## Technical Configuration Details

- Source code remains "Express" (not separate GLS code)
- Argentina has similar setup but GLS raised concerns about code changes
  - Express sends as "XP bulk" format
  - GLS was sending as "XP via" format
  - Need consistent approach discussion with Krishna
- Expiry date handling: can send as null (Flex defaults to 2030 or 2300)
- Volume migration will be phased, not immediate switch

## Action Items

- [ ] Float account discussion with Nanirajan (missed due to absence) — Day zero approach: Excel sheet from CDP team to Express; Phase 2: mapping transformation
- [ ] Deepak — work with Niranjan and Krishna for earmark publisher ICD documentation
- [ ] Validate special character handling in address line 1
  - Testing discrepancy between real-time and batch processing
  - Validate with Hari on any EOD file changes
  - Sign-off expected by Monday/Tuesday after batch validation
