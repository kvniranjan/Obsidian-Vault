---
date: 2026-04-01
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - float-account
  - express
  - amcar
---
# Float Account Payments Approach for Brazil Onboarding

**Date:** 2026-04-01
**Projects:** [[FlexCube Brazil Payments]], [[Amcar Integration]]

## Float Account Payment Routing — Approach Decision

- Two solutions proposed for Express onboarding to Brazil (float account support):
  1. Enhance existing [[Amcar Integration|AM-CAR]] handoff with float account details → Express subscribes via ISD Cloud
  2. Online notification from Flex on every mapping creation/modification/closure → partner (AM-CAR or Express) consumes and stores locally
- **Approach 2 is the recommended option** (endorsed by Arun, Ollie, and the broader team)
- Approach 1 (EOD NDM file via Payment Hub/GPP route) explicitly ruled out — file-based route not recommended
- Outstanding ambiguity: whether the online notification goes to Express directly or to AM-CAR — not yet confirmed
  - Trina confirmed yesterday this is still unresolved on Express's side
  - Express prefers Kafka-based approach; resistant to older/existing feed methods
- Swapnil raised concerns about the CAP service build required for online triggering — resource-intensive, updates are rare
  - No resolution on this concern received; team lost track of it over the past week

## Blind Key Requirement (EPIC Countries)

- Blind key restricts Checker from viewing Maker-inputted fields during journal entry authorization
- Four masked fields: account, amount, currency, value date
- Applies to: single entry detail screen, multi-entry detail screen, summary screen
- Already live in Nimia; rollout now scoped for EPIC countries
- L2 review completed — approach approved by the group

## Action Items

- [ ] Giri — connect with Swapnil to confirm his alignment on Approach 2; share update once confirmed
- [ ] Niranjan — once Giri confirms Swapnil's sign-off, update design doc with full Approach 2 details (XML tags etc.)
- [ ] Niranjan — retain Approach 1 in the document under alternatives/considered approaches
- [ ] Niranjan — share updated design doc for offline review
- [ ] Niranjan — clarify with Naresh/Express whether online notification goes to Express or AM-CAR
- [ ] Akash — arrange meeting between relevant parties (float account / GPP topic follow-up)
