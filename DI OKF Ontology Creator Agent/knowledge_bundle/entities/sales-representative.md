---
title: Sales Representative
concept_type: entity
business_domain: sales-organization
technical_mapping: dim_sales_rep
keys:
  primary_key: sales_rep_key
  business_key: rep_id
---

# Sales Representative

## Business Definition
Sales representative dimension representing the sales owner and organizational assignment associated with a booking.

## Technical Mapping
- Table: `dim_sales_rep`
- Primary Key: `sales_rep_key`
- Business Key: `rep_id`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Sales Representative Key | `sales_rep_key` | Surrogate key that uniquely identifies a sales representative record. |
| Sales Representative ID | `rep_id` | Business identifier assigned to a sales representative. |
| Sales Representative Name | `rep_name` | Name of the sales representative associated with the booking. |
| Sales Role | `sales_role` | Role performed by the sales representative in the selling process. |
| Sales Team | `sales_team` | Organizational sales team to which the representative belongs. |
| Segment Covered | `segment_covered` | Customer segment or market coverage assigned to the sales representative. |

## Keys

- Primary Key: `sales_rep_key`
- Business Key: `rep_id`

## Measures

This entity does not contain explicit stored measures. It contextualizes [Booking Amount USD](../measures/booking-amount-usd.md), [Quantity Sold](../measures/quantity-sold.md), and [Discount Percentage](../measures/discount-percentage.md).

## Relationships

- [Sales Representative to Booking Transaction](../relationships/sales-representative-to-booking-transaction.md)

## Related Concepts

- [Sales Organization Domain](../domains/sales-organization.md)
- [Booking Transaction](booking-transaction.md)
