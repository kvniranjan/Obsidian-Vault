---
date: 2026-03-20
projects:
  - GL Reclassification
  - QFI-FlexCube Integration
tags:
  - meeting
  - flexcube
  - seccor
  - gl
  - earmarking
---
# FlexCube and SecCor Integration: GL Handoffs and Earmarking Workflow

**Date:** 2026-03-20
**Projects:** [[GL Reclassification]], [[QFI-FlexCube Integration]]

## GL Handoff Mapping & Validation

- Richard from FlexTip analyzing GL movements from Roberto's example
- Mapped movements to SecCor (green) and FlexCube (salmon) handoffs
  - Reserve posting and transitory movements identified
  - Two tax-related accounts (IOF tax) not in original example
  - Wash movement combines three separate postings (client movement + tax + cash concentration)
- All movements appear in opposite direction to entitlement processing
  - Need Finance/Operations confirmation on expected GL posting direction
  - FlexTip tech team cannot validate financial logic

## Outstanding Requirements & Clarifications

- Missing tax movement example from Roberto
  - Need sample showing tax on entitlement scenarios
  - IOF tax entries sent regardless of applicability (zero amounts)
- Finance team involvement required
  - Schedule dedicated call with Finance participation
  - Validate GL posting directions and requirements
  - Confirm which entries need handoff transmission

## Non-Impact Testing Status

- Pending ticket with FullSuite Finance team
- Testing managed by Change Management team, not FlexTip tech
- Contact testing coordinator listed in JIRA for next steps
- No development changes expected

## Earmarking Design Updates

- Flow significantly changed from original proposal
- GCCS-FlexCube earmarking cache still required
- Refined version to be shared early next week
- Volume planning needed once approach finalized
  - Select transactions only (rights events, priority offers)
  - GCCS will specify earmarking requests

## Master Data File (MDF) Integration

- SecCor currently uses Cosmos accounts, looks up MDF for actual DDA accounts
- Two options under review:
  1. Enhance existing SecCor-to-CP2 handoff with MDF details
  2. Send MDF directly from FlexCube to CP2
- FlexCube sees no technical blockers for option 2
  - Requires architect forum approval
  - Similar to existing SecCor file, just additional partner

## Cash Statement Generation

- FlexCube continues sending cash postings without free text
- CP2 adds enrichment text during statement generation
- Need to confirm CP2 feed mechanism (likely NDM)
  - SecCor and CP2 share mainframe logical partition
  - Casa integration possible if NDM confirmed

## Action Items

- [ ] Schedule Finance team call for GL direction validation
- [ ] Check JIRA testing coordinator for non-impact test status
- [ ] Request 2025 entitlement volumes (not just event counts)
- [ ] Confirm CP2 feed mechanism with Ed
- [ ] Share refined earmarking flow early next week
