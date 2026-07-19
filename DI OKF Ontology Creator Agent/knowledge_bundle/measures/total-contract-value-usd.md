---
title: Total Contract Value USD
concept_type: measure
aggregation_type: sum
technical_mapping: fact_bookings.tcv_usd
related_entities:
  - booking-transaction
related_domains:
  - sales-bookings
---

# Total Contract Value USD

## Business Definition
Total contract value in US dollars associated with the booking. For subscription and SaaS offers, the booking amount equals total contract value.

## Aggregation Type
Sum

## Related Entities

- [Booking Transaction](../entities/booking-transaction.md)

## Related Domains

- [Sales Bookings](../domains/sales-bookings.md)
- [Customer](../domains/customer.md)
- [Product](../domains/product.md)
- [Contract](../domains/contract.md)
- [Time](../domains/time.md)
