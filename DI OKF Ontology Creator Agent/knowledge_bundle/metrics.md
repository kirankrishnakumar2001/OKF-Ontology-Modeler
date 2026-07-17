---
title: Semantic Metrics
subject_area: Cisco Sales Bookings and Revenue Analytics
status: validated-with-warnings
---

# Semantic Metrics

## Overall Metrics

| Metric | Value |
| --- | --- |
| Total Domains | 8 |
| Total Entities | 8 |
| Total Relationships | 9 |
| Total Measures | 6 |
| Total Glossary Terms | 53 |
| Explicit Relationships | 7 |
| Inferred Relationships | 2 |
| Validation Status | Validated with warnings |

## Per-Domain Metrics

| Domain Name | Entity Count | Measure Count | Related Relationships | Domain Status |
| --- | --- | --- | --- | --- |
| Sales Bookings | 1 | 6 | 7 explicit | Structurally complete; data unavailable |
| Customer | 1 | 0 | 1 explicit, 1 inferred | Structurally complete; data unavailable |
| Product | 1 | 0 | 1 explicit, 1 inferred | Structurally complete; data unavailable |
| Partner / Channel | 1 | 0 | 1 explicit | Structurally complete; data unavailable |
| Geography | 1 | 0 | 1 explicit, 1 inferred | Structurally complete; data unavailable |
| Sales Organization | 1 | 0 | 1 explicit | Structurally complete; data unavailable |
| Contract | 1 | 0 | 1 explicit, 1 inferred | Structurally complete; data unavailable |
| Time | 1 | 0 | 1 explicit | Structurally complete; data unavailable |

## Measure Inventory

| Measure | Aggregation Type | Related Entity | Related Domain |
| --- | --- | --- | --- |
| Quantity Sold | Sum | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |
| Unit List Price USD | Sum, Avg | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |
| Discount Percentage | Avg | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |
| Booking Amount USD | Sum | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |
| Annual Contract Value USD | Sum | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |
| Total Contract Value USD | Sum | [Booking Transaction](entities/booking-transaction.md) | [Sales Bookings](domains/sales-bookings.md) |

## Validation Warnings

- Source-system row counts were reported as zero, so data-quality and value-domain profiling could not be completed.
- `booking_type`, `is_renewal`, `auto_renew_flag`, and some contextual associations remain partially inferred.
- Inferred relationships are documented separately from explicit dimensional foreign-key relationships.
