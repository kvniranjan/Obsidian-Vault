---
date: 2026-04-02
project: FlexCube Brazil Payments
tags:
  - meeting
  - brazil
  - argentina
  - earmarking
  - flexcube
  - c900
---
# Partial Earmark Process for Argentina and Brazil Banking Systems

**Date:** 2026-04-02
**Project:** [[FlexCube Brazil Payments]]

## Partial Earmark — Core Problem

- [[FlexCube Brazil Payments|FlexCube]] doesn't store credit line (DOL) data for non-HVA accounts — that sits in C900
- Balance inquiry from FlexCube returns available balance only, not DOL utilization
- Partial earmark logic: on NSF response, query available balance → amend amount → re-submit earmark
  - Works in regions where one system holds both balance and credit line (APAC, EMEA RBCs)
  - Breaks in LATAM because two separate systems handle balance (FlexCube) vs. limits (C900)

## HVA vs. Non-HVA Architecture

- HVA accounts: daily feed from C900 pushed into FlexCube tables; FlexCube has limit data
- Non-HVA accounts: FlexCube sends transaction amount + account number to C900 → receives ACK/NACK only (no balance or DOL figure returned)
- Argentina currently: pure pass-through to FlexCube, no balance inquiry step today
- Brazil: same C900 ACK/NACK mechanism as Argentina; no DOL balance returned

## Partial Earmark Rollout Scope

- Partial earmark is a default/standard offering for all CPX onboardings — already in scope for Argentina
- Product requirement: payments should not be stuck on NSF; use whatever balance is available
- Should be reviewed for all LATAM (Brazil + Argentina at minimum), not Argentina alone
- BCR program countries (moving to Pismo/Clue) are a separate track — leave aside for now

## C900 Integration Gap

- GLS does not currently connect to C900
- C900 is an approval system, not a balance-publishing system — no known API to return DOL balance on query
- Strategic direction: DOL/facility data eventually moves to Clue (Helios + Clue replacing C900), but not in scope for Argentina now
- Moving all facility data to Clue would require significant rework — not a near-term option

## Design Options Discussed

- **Option A:** Orchestrate between FlexCube (balance) and C900 (DOL) — raises performance concerns; frequency of NSF scenarios unknown
- **Option B:** Enhance C900 interface to return DOL balance (not just ACK/NACK) — needs C900 team engagement to confirm feasibility
- **Option C:** Publish DOL data from C900 into FlexCube tables (similar to HVA feed) — noted but no owner
- No decision reached; team to go back to drawing board

## Open Questions

- How frequently do NSF scenarios occur in LATAM? (No data available; Shanta to check with local team)
- Does C900 have an API that returns DOL/limit balance on account query?
- Who is the C900 contact/owner? (Ashwathi to check; will share in chat)
- CAP team building a query to get balances — input is account number only; need to confirm exact interface spec

## Action Items

- [ ] Shanta — check with local Argentina/Brazil team for NSF frequency data
- [ ] Shanta — discuss design options internally with the team
- [ ] Arun / Technical leads — arrange internal call with CAP and FlexCube team (Monday, same time; Ashish to join)
- [ ] Arun / Technical leads — confirm exact interface spec between FlexCube and C900 (MQ-based API call — confirm fields sent/returned)
- [ ] Ashwathi — find C900 team contact and share in chat
- [ ] All — engage C900 team to assess whether a balance/DOL query API exists or can be built
- [ ] All — schedule follow-up call after internal review and C900 engagement
