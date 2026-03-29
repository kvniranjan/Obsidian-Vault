---
date: 2026-03-06
project: QFI-FlexCube Integration
tags:
  - meeting
  - brazil
  - flexcube
  - qfi
  - uat
---
# QFI and FlexCube Integration Phase One

**Date:** 2026-03-06
**Project:** [[QFI-FlexCube Integration]]

## Announcements
- Project timeline separated into two phases due to consent order requirements
  - Phase one delivery target: May production rollout
  - Phase two implementation: November completion
- Current production system (Evox/Ebooks) will be retired and replaced with QFI implementation for fixed income products (buy, sell, repos, reverse repos)

## Review of Progress
- Phase one scope has been finalized and locked to meet consent order deadlines
  - QFI will use same GL account flow as Ebooks currently configured in Flex
  - Query balance functionality will be handled by FWS through existing XML file interface
  - Transaction posting will use new JSON Kafka model for QFI system integration
- UAT environment setup nearly complete with plans to go online this week
  - Source code implementation in UAT configured to receive QFI postings
  - Technical documentation and interface specifications have been exchanged between teams

## Key Achievements
- Technical agreements and documentation finalized for phase one implementation
- Multiple technical discussions completed to resolve integration approach differences
- Mock data and interface comparisons successfully analyzed and shared
- Team alignment achieved on using Brazil-specific implementation model rather than APAC/EMEA approach

## Challenges
- Integration model confusion between QFI team expectations and Flex implementation
  - QFI team expected to use same approach as other regions (APAC/EMEA)
  - Flex clarified that Brazil uses different database structure requiring JSON Kafka model
  - Cannot implement APAC/EMEA customer DDA movement approach due to technical constraints
- Miscommunication identified regarding online transaction posting requirements
  - QFI team unclear on inter-system shell requirements for online vs batch processing
- Phase two implementation may impact existing reconciliation and DDA processes

## Action Items
- [ ] Reschedule technical clarification meeting for Monday or Tuesday (Fernando to coordinate)
- [ ] Configure QFI source code in Flex UAT environment using Ebooks account path (Jefferson/Flex team) — Target: Thursday
- [ ] Review and share technical documentation again (Flex team to Fernando)
- [ ] Proceed with UAT setup without further delays while technical details are clarified separately
