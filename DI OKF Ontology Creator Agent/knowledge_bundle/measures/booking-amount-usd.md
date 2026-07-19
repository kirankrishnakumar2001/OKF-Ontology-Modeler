---
title: Booking Amount USD
concept_type: measure
aggregation_type: sum
technical_mapping: fact_bookings.booking_amount_usd
related_entities:
  - booking-transaction
related_domains:
  - sales-bookings
---

# Booking Amount USD

## Business Definition
Net booked monetary value in US dollars for the booking line. This is the headline bookings KPI and the governed measure for total bookings reporting.

## Aggregation Type
Sum

## Related Entities

- [Booking Transaction](../entities/booking-transaction.md)

## Related Domains

- [Sales Bookings](../domains/sales-bookings.md)
- [Customer](../domains/customer.md)
- [Product](../domains/product.md)
- [Partner / Channel](../domains/partner-channel.md)
- [Geography](../domains/geography.md)
- [Sales Organization](../domains/sales-organization.md)
- [Contract](../domains/contract.md)
- [Time](../domains/time.md)
