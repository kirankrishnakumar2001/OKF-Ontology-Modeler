---
title: Booking Transaction
concept_type: entity
technical_mapping: fact_bookings
domain: ../domains/sales-bookings.md
measures:
  - ../measures/quantity-sold.md
  - ../measures/unit-list-price-usd.md
  - ../measures/discount-percentage.md
  - ../measures/booking-amount-usd.md
  - ../measures/annual-contract-value-usd.md
  - ../measures/total-contract-value-usd.md
relationships:
  - ../relationships/date-to-booking-transaction.md
  - ../relationships/customer-to-booking-transaction.md
  - ../relationships/product-to-booking-transaction.md
  - ../relationships/partner-to-booking-transaction.md
  - ../relationships/geography-to-booking-transaction.md
  - ../relationships/sales-representative-to-booking-transaction.md
  - ../relationships/contract-to-booking-transaction.md
---

# Booking Transaction

## Business Definition

Central fact entity storing booking transactions at one booking transaction or order-line booking event grain, with commercial measures and dimensional references.

## Technical Mapping

- Table: `fact_bookings`
- Entity Type: Fact
- Primary Key: `booking_id`
- Foreign Keys: `date_key`, `customer_key`, `product_key`, `partner_key`, `geography_key`, `sales_rep_key`, `contract_key`
- Business Keys: `booking_id`; operational grouping fields `order_number`, `order_line_number`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Booking ID | `booking_id` | Unique identifier for a booking transaction record. |
| Order Number | `order_number` | Customer or partner order number associated with the booking. |
| Order Line Number | `order_line_number` | Line item number within the order. |
| Booking Date Key | `date_key` | Link to the reporting date. |
| Customer Key | `customer_key` | Link to the customer account. |
| Product Key | `product_key` | Link to the sold product or offer. |
| Partner Key | `partner_key` | Link to the partner involved in the sale. |
| Geography Key | `geography_key` | Link to sales geography. |
| Sales Representative Key | `sales_rep_key` | Link to the responsible sales representative. |
| Contract Key | `contract_key` | Link to associated contract context. |
| Booking Type | `booking_type` | Classification of the booking event such as New, Renewal, or Upsell. |
| Renewal Indicator | `is_renewal` | Indicator showing whether the booking is related to a contract renewal. |

## Keys

- Primary Key: `booking_id`
- Foreign Key: `date_key` -> [Date](date.md)
- Foreign Key: `customer_key` -> [Customer](customer.md)
- Foreign Key: `product_key` -> [Product](product.md)
- Foreign Key: `partner_key` -> [Partner](partner.md)
- Foreign Key: `geography_key` -> [Geography](geography.md)
- Foreign Key: `sales_rep_key` -> [Sales Representative](sales-representative.md)
- Foreign Key: `contract_key` -> [Contract](contract.md)

## Measures

- [Quantity Sold](../measures/quantity-sold.md)
- [Unit List Price USD](../measures/unit-list-price-usd.md)
- [Discount Percentage](../measures/discount-percentage.md)
- [Booking Amount USD](../measures/booking-amount-usd.md)
- [Annual Contract Value USD](../measures/annual-contract-value-usd.md)
- [Total Contract Value USD](../measures/total-contract-value-usd.md)

## Relationships

- [Date to Booking Transaction](../relationships/date-to-booking-transaction.md)
- [Customer to Booking Transaction](../relationships/customer-to-booking-transaction.md)
- [Product to Booking Transaction](../relationships/product-to-booking-transaction.md)
- [Partner to Booking Transaction](../relationships/partner-to-booking-transaction.md)
- [Geography to Booking Transaction](../relationships/geography-to-booking-transaction.md)
- [Sales Representative to Booking Transaction](../relationships/sales-representative-to-booking-transaction.md)
- [Contract to Booking Transaction](../relationships/contract-to-booking-transaction.md)

## Related Concepts

- Domain: [Sales Bookings](../domains/sales-bookings.md)
- Process context: Quote-to-Booking
- KPI context: Total Bookings, Net-New vs Renewal mix, ACV / TCV, Partner contribution
