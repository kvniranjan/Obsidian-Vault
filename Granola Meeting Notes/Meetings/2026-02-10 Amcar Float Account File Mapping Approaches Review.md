---
date: 2026-02-10
project: Amcar Integration
tags:
  - meeting
  - brazil
  - amcar
  - file-mapping
  - float-account
---
# Amcar Float Account File Mapping Approaches Review

**Date:** 2026-02-10
**Project:** [[Amcar Integration]]

## Two Approaches Under Consideration

### Approach 1: Enhance Existing File (Recommended)
- Add 4 new fields to current Amcar handoff file (end-of-day)
- Uses existing file structure, minimal logic changes
- Only Amcar uses this file (no impact on other systems)
- File layout change needed

### Approach 2: Reuse Payment Hub File
- Send same file currently sent to payment hub directly to Amcar
- No changes required on sender side
- Amcar must join/reconcile two different files
- Currently XML format, Amcar needs JSON

## Decision
- Team recommends Approach 1 — easier implementation overall, avoids complex reconciliation at Amcar
- Need to inform Amcar of potential approach change from previous alignment

## Action Items
- [ ] Add recommendation comments to shared document
- [ ] Inform Amcar of approach change from previous alignment
