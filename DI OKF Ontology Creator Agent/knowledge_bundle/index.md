---
title: Cisco Bookings OKF Knowledge Bundle
concept_type: knowledge_bundle_index
domains:
  - sales-bookings
  - customer
  - product
  - partner-channel
  - geography
  - sales-organization
  - contract
  - time
entities:
  - booking-transaction
  - customer
  - product
  - partner
  - geography
  - sales-representative
  - contract
  - date
measures:
  - quantity-sold
  - unit-list-price-usd
  - discount-percentage
  - booking-amount-usd
  - annual-contract-value-usd
  - total-contract-value-usd
---

# Cisco Bookings OKF Knowledge Bundle

This Open Knowledge Format knowledge bundle captures the Cisco Sales Bookings and Revenue Analytics semantic model derived from the validated OSI semantic model and enriched by the Cisco quote-to-booking business process document.

## Navigation

- [Semantic Summary](semantic_summary.md)
- [Metrics](metrics.md)
- [Domains](domains/index.md)
- [Entities](entities/index.md)
- [Relationships](relationships/index.md)
- [Measures](measures/index.md)
- [Glossary](glossary/index.md)

## Business Context

The model represents a star-schema analytical foundation centered on booking transactions at order-line grain. It supports governed analysis of bookings, ACV, TCV, quantity, discounting, customer segmentation, product mix, partner contribution, geography, sales ownership, contract context, and fiscal reporting.

## Validation Notes

- OSI Semantic Model readability: Pass
- Business Process document readability: Pass
- Duplicate entities: None detected
- Duplicate domains: None detected
- Missing relationships: No missing explicit fact-to-dimension relationships detected
- Warnings: inferred semantic associations remain confidence-scored and separate from explicit foreign-key relationships
