---
title: Booking Transaction
concept_type: entity
business_domain: sales-bookings
technical_mapping: fact_bookings
keys:
  primary_key: booking_id
  foreign_keys:
    - date_key
    - customer_key
    - product_key
    - partner_key
    - geography_key
    - sales_rep_key
    - contract_key
---

# Booking Transaction

## Business Definition
Central fact entity storing booking transactions at one booking transaction / order-line booking event grain with commercial measures and dimensional references.

## Technical Mapping
- Table: `fact_bookings`
- Grain: one booking transaction / order-line booking event
- Operational grouping: `order_number`, `order_line_number`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Booking ID | `booking_id` | Unique identifier for a booking transaction record. |
| Order Number | `order_number` | Customer or partner order number associated with the booking. |
| Order Line Number | `order_line_number` | Line item number within the order. |
| Booking Date Key | `date_key` | Foreign key linking the booking to the reporting date. |
| Customer Key | `customer_key` | Foreign key linking the booking to the customer account. |
| Product Key | `product_key` | Foreign key linking the booking to the sold product or offer. |
| Partner Key | `partner_key` | Foreign key linking the booking to the partner involved in the sale. |
| Geography Key | `geography_key` | Foreign key linking the booking to sales geography. |
| Sales Representative Key | `sales_rep_key` | Foreign key linking the booking to the responsible sales representative. |
| Contract Key | `contract_key` | Foreign key linking the booking to associated contract context. |
| Booking Type | `booking_type` | Classification of the booking event by commercial motion such as New, Renewal, or Upsell. |
| Renewal Indicator | `is_renewal` | Indicator showing whether the booking is related to a contract renewal. |

## Keys

- Primary Key: `booking_id`
- Foreign Keys: `date_key`, `customer_key`, `product_key`, `partner_key`, `geography_key`, `sales_rep_key`, `contract_key`

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

- [Sales Bookings Domain](../domains/sales-bookings.md)
- [Customer](customer.md)
- [Product](product.md)
- [Partner](partner.md)
- [Geography](geography.md)
- [Sales Representative](sales-representative.md)
- [Contract](contract.md)
- [Date](date.md)
