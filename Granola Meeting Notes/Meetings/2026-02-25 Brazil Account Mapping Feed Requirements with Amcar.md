---
date: 2026-02-25
project: Amcar Integration
tags:
  - meeting
  - brazil
  - amcar
  - flexcube
  - account-mapping
---
# Brazil Account Mapping Feed Requirements with Amcar

**Date:** 2026-02-25
**Project:** [[Amcar Integration]]

## Flex-Amcar Integration Challenge
- Flex cannot add 4 additional float account mapping attributes to existing customer/account feeds
  - Current services only support core customer (STTM_CUSTOMER) and account (HTTM_CUST_ACCOUNT) data
  - Mapping data maintained outside core customer/account maintenance
  - New service would require DAC approval (currently rejected)
- Impact concerns for other product processors consuming same feeds

## Alternative Approaches Discussed
- Redirect existing NDM file from Flex to Amcar (currently goes to GPPSP)
- CPX direct consumption from existing Flex feed
- Country-specific customization at Amcar level (Brazil-only, not global standard)

## Architecture Context
- Target state: AMS -> E-Sales -> ISG Cloud (no Flex dependency)
- Current: Flex -> Amcar -> ISG Cloud -> CPX
- Future: AMS -> Vanguard for payment ecosystems
- CPX code already in production based on Amcar commitments

## Action Items
- [ ] Escalate to services senior leadership for collective decision
- [ ] Praveen: Send meeting minutes and coordinate offline discussion
- [ ] Decision required on existing feed redirection vs alternative solution (April release testing starting Monday)
