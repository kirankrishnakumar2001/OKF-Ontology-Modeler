---
title: Sales Bookings
concept_type: domain
slug: sales-bookings
related_entities:
  - booking-transaction
related_measures:
  - quantity-sold
  - unit-list-price-usd
  - discount-percentage
  - booking-amount-usd
  - annual-contract-value-usd
  - total-contract-value-usd
---

# Sales Bookings

## Description
Central transactional domain capturing booking events at order-line grain and the measures used for bookings analytics.

## Business Purpose
Measure demand, bookings performance, renewal mix, and contract value. This domain anchors the quote-to-booking process where a valid accepted order becomes a booking and is classified as New, Renewal, or Upsell.

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
