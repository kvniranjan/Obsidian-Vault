---
date: 2026-03-02
project: ECS Plus Partner Integration
tags:
  - meeting
  - ecs-plus
  - uat
  - deployment
  - brazil
---
# UAT Deployment Approval for ECS Plus Partner Services

**Date:** 2026-03-02
**Project:** [[ECS Plus Partner Integration]]

## ECS Plus Partner Integration Services
- Two services require UAT deployment for ECS Plus partner onboarding
  - EOD SOD notification service (enhanced to send JSON to ECS Plus via Kafka)
  - Transaction posting service (new instance using existing Express codebase)
- Development completed, both services ready for deployment
- Current freeze period requires exceptional approval

## Deployment Dependencies & Approvals
- CQE approval needed first before seeking exceptional approval
  - Priya to review unit test results and provide confirmation
  - Gopi to share unit test results (local testing sufficient)
- Exceptional approval required due to current freeze
  - Magali to handle exceptional approval process
  - Timeline: 1 day code drop + couple days sanity testing
- No impact expected on existing flows — code base isolated

## Technical Implementation
- EOD SOD service: existing XML flow unchanged, added JSON conversion for ECS Plus via Kafka
- Transaction posting service: new Helm chart with ECS Plus configuration, separate instance
- Duplicate check constraints available in database
- One CV environment available for testing

## Action Items
- [ ] Priya: Review DAG and issue CQE approval in email thread
- [ ] Gopi: Share unit test results for CQE review
- [ ] Magali: Seek exceptional approval after CQE confirmation
- [ ] Niranjan: Follow up with UV on [[QFI-FlexCube Integration]] source code feedback
- [ ] Shiva: Confirm March release impact after 10:30 sync call
