---
date: 2026-03-30
project: FlexCube Brazil Payments
tags:
  - meeting
  - defect
  - special-characters
  - uat
  - h1b
---
# Customer Name Special Character Issue and H1B Discussion

**Date:** 2026-03-30
**Project:** [[FlexCube Brazil Payments]]

## Technical Issue Investigation

- Customer name field displaying incorrectly in system
  - Frontend shows different value than backend database
  - Special character parsing issue identified in Flex system
  - XML receiving correct data but database missing special characters
- Root cause analysis needed
  - Database trimming logic affecting customer name field
  - Address fields working properly with special characters
  - Issue appears specific to customer name column

## System Comparison & Data Flow

- Handoff system vs. notification system discrepancy
  - Same source system (Flex) generating different outputs
  - CDP pulling different data than XML receives
  - Need to investigate RAD level processing
- Testing limitations
  - UAT environment currently down
  - OpenShift network issues preventing validation
  - Cannot test baseline scenarios until environment restored

## H1B Lottery Status

- Application submitted without employee notification — all employees automatically entered in lottery
- Outcome uncertain, no clear communication from company
- Worst case scenario planning needed if not selected
- Documentation requirements unclear; timeline and next steps undefined

## Action Items

- [ ] Assign defect to Niranjan for investigation
- [ ] Update defect tracking with findings
- [ ] Schedule follow-up call once UAT environment restored
- [ ] Test baseline scenarios with 20-character vs. 27-character limits
- [ ] Investigate database trimming logic at system level
