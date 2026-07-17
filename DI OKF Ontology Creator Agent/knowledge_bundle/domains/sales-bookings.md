---
title: Sales Bookings
concept_type: domain
bundle: Cisco Sales Bookings and Revenue Analytics
related_entities:
  - ../entities/booking-transaction.md
related_measures:
  - ../measures/quantity-sold.md
  - ../measures/unit-list-price-usd.md
  - ../measures/discount-percentage.md
  - ../measures/booking-amount-usd.md
  - ../measures/annual-contract-value-usd.md
  - ../measures/total-contract-value-usd.md
related_relationships:
  - ../relationships/date-to-booking-transaction.md
  - ../relationships/customer-to-booking-transaction.md
  - ../relationships/product-to-booking-transaction.md
  - ../relationships/partner-to-booking-transaction.md
  - ../relationships/geography-to-booking-transaction.md
  - ../relationships/sales-representative-to-booking-transaction.md
  - ../relationships/contract-to-booking-transaction.md
---

# Sales Bookings

## Description
Central transactional domain capturing booking events at order-line grain and the measures used for bookings analytics.

## Business Purpose
Measures demand, bookings performance, renewal mix, and contract value. The business process states that a booking is recorded when Cisco accepts a valid order with committed value, making this domain the core analytical anchor for demand reporting.

## Related Entities
- [Booking Transaction](../entities/booking-transaction.md)

## Related Measures
- [Quantity Sold](../measures/quantity-sold.md)
- [Unit List Price USD](../measures/unit-list-price-usd.md)
- [Discount Percentage](../measures/discount-percentage.md)
- [Booking Amount USD](../measures/booking-amount-usd.md)
- [Annual Contract Value USD](../measures/annual-contract-value-usd.md)
- [Total Contract Value USD](../measures/total-contract-value-usd.md)

## Related Relationships
- [Date to Booking Transaction](../relationships/date-to-booking-transaction.md)
- [Customer to Booking Transaction](../relationships/customer-to-booking-transaction.md)
- [Product to Booking Transaction](../relationships/product-to-booking-transaction.md)
- [Partner to Booking Transaction](../relationships/partner-to-booking-transaction.md)
- [Geography to Booking Transaction](../relationships/geography-to-booking-transaction.md)
- [Sales Representative to Booking Transaction](../relationships/sales-representative-to-booking-transaction.md)
- [Contract to Booking Transaction](../relationships/contract-to-booking-transaction.md)
