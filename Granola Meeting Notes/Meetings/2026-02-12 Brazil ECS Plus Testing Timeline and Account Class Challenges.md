---
date: 2026-02-12
project: ECS Plus Partner Integration
tags:
  - meeting
  - brazil
  - ecs-plus
  - uat
  - account-class
  - testing
---
# Brazil ECS Plus Testing Timeline and Account Class Challenges

**Date:** 2026-02-12
**Project:** [[ECS Plus Partner Integration]]

## UAT Timeline & Dependencies
- UAT testing start date: February 23rd
- April release sign-off: March 13th — only 2 weeks for development (extremely tight)
- Testing constraints:
  - Can start API testing but not end-to-end without PAT template
  - Downstream testing (FF Full Suite) cannot proceed without complete setup
  - March release (Feb 21 - March 6) creates environment conflicts

## Account Class Configuration Risks
- Primary blocker: PAT template still pending
- Two approaches:
  1. Use existing ESCAN account (requires business owner approval)
  2. Create new account class (high risk — not feasible within one week)
- Recommendation: Proceed with existing account class, defer changes to Phase 2

## MIS Code Setup Confusion
- Brazil uses GO codes instead of MIS codes (unlike APAC/EMEA)
- Current setup uses GO code 1585 (BR Cards specific)
- Downstream impact: CDP filters based on MIS code 9988; ECS Plus has validation checks
- Waiting for direction on identifier approach

## Team Availability
- Gopi (CIP): On leave next week, Amit Jain covering
- Code ready by February 23rd target
- NFT timeline: 2 weeks starting March 6th (post-functional testing)

## Action Items
- [ ] CQE: FS document approval, Story ID creation, Release notes
- [ ] Niranjan: Provide upstream partner details for CQE
- [ ] Determine account class approach before UAT begins
