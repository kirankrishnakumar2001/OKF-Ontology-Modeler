---
title: Sales Representative
concept_type: entity
technical_table_name: dim_sales_rep
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/sales-organization.md
related_relationships:
  - ../relationships/sales-representative-to-booking-transaction.md
---

# Sales Representative

## Business Definition
Sales representative dimension representing the sales owner and organizational assignment associated with a booking.

## Technical Mapping
- Technical Table: `dim_sales_rep`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
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
- No explicit measures are modeled for this entity.

## Relationships
- [Sales Representative to Booking Transaction](../relationships/sales-representative-to-booking-transaction.md)

## Related Concepts
- Domain: [Sales Organization](../domains/sales-organization.md)
- Related entity: [Booking Transaction](booking-transaction.md)
