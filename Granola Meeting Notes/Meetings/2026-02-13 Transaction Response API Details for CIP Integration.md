---
date: 2026-02-13
project: ECS Plus Partner Integration
tags:
  - meeting
  - cip
  - api
  - brazil
  - ecs-plus
---
# Transaction Response API Details for CIP Integration

**Date:** 2026-02-13
**Project:** [[ECS Plus Partner Integration]]

## API Response Structure
- Need detailed specifications for CIP transaction posting responses
- Current system handles two-leg transactions with three response levels:
  - Individual leg responses
  - Transaction-level response
  - Final consolidated response
- JSON format will mirror existing XML structure from Flex

## NSF and Rejection Code Specifications
- Require unique rejection codes for two categories:
  1. Non-sufficient funds (NSF) — exclusive identification needed
  2. All other rejections — consolidated under single category
- Need specific error codes and status descriptions for LATAM region
  - EMEA and APAC already have established codes

## Error Handling
- When one leg succeeds but transaction still rejected: need to identify which specific leg failed
- Sample responses needed for: invalid account, NSF, successful, and mixed scenarios

## Technical Specifications
- Response byte format confirmation needed (3-byte vs 4-byte)
- Duplicate check: generic "duplicate reference number" message expected
- Go code confirmation resolved (was previously 9988 code)

## Action Items
- [ ] Niranjan: Share current BAU response JSON samples, specific error codes, debit posting layout mapping
- [ ] Application team development blocked pending these samples
- [ ] Request topic creation dependent on cash account operations approval
