---
title: Sales Representative
concept_type: entity
technical_mapping: dim_sales_rep
domain: ../domains/sales-organization.md
relationships:
  - ../relationships/sales-representative-to-booking-transaction.md
---

# Sales Representative

## Business Definition

Sales representative entity representing the sales owner and organizational assignment associated with a booking.

## Technical Mapping

- Table: `dim_sales_rep`
- Entity Type: Dimension
- Primary Key: `sales_rep_key`
- Business Key: `rep_id`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Sales Representative Key | `sales_rep_key` | Surrogate key uniquely identifying a sales representative record. |
| Sales Representative ID | `rep_id` | Business identifier assigned to a sales representative. |
| Sales Representative Name | `rep_name` | Name of the sales representative associated with the booking. |
| Sales Role | `sales_role` | Role performed by the sales representative. |
| Sales Team | `sales_team` | Organizational sales team to which the representative belongs. |
| Segment Covered | `segment_covered` | Customer segment or market coverage assigned to the representative. |

## Keys

- Primary Key: `sales_rep_key`
- Business Key: `rep_id`

## Measures

- None explicit.

## Relationships

- [Sales Representative to Booking Transaction](../relationships/sales-representative-to-booking-transaction.md)

## Related Concepts

- Domain: [Sales Organization](../domains/sales-organization.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
