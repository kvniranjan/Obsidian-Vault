---
date: 2026-02-26
project: ECS Plus Partner Integration
tags:
  - meeting
  - brazil
  - ecs-plus
  - uat
  - cash-account
  - cip
---
# Brazil Cash Account Configuration and UAT Testing

**Date:** 2026-02-26
**Project:** [[ECS Plus Partner Integration]]

## Legal & Account Configuration
- Legal confirmed PND cannot be applied to cash accounts in Brazil
  - Alternative options like X Scroll available but not preferred
- Current dilemma: Standard cash account vs guardian account
  - Both require business owner alignment for local regulatory compliance
- Matilda seeking formal legal confirmation on proposed approach

## Testing Strategy & Timeline
- Agreement reached to test basic flows while finalizing account configuration
  - Use standard cash account for end-to-end validation
  - Validate data flow from FlexCube to calendars team
- Major blocker: Global code freeze until March 8th
  - CIP code not yet deployed to UAT environment
  - Only regulatory exceptions allowed during freeze period
- Testing dependencies:
  - FlexCube testing expected to complete by tomorrow
  - CQE environment availability from March 2nd
  - FFS deadline: March 23rd for April release (critical)

## Technical Challenges
- Need GL account and account class definition before UAT
- Local tax implications (IOF) for Brazil operations
- Code deployment status:
  - EVOD notification deployed before freeze
  - Transaction posting service awaiting deployment
  - CIP services ready but blocked by freeze

## Action Items
- [ ] Internal meeting with CQE, developers, and Nan for exception request assessment
- [ ] Matilda: Finalize account class decision with business stakeholders
- [ ] Niranjan: Follow up on CQE environment availability, FFS timeline (March 23rd), A5 and GDR/CM realignment
