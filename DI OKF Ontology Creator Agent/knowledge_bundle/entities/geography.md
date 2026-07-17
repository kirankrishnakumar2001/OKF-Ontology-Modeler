---
title: Geography
concept_type: entity
technical_table_name: dim_geography
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/geography.md
related_relationships:
  - ../relationships/geography-to-booking-transaction.md
  - ../relationships/customer-headquarters-to-geography.md
---

# Geography

## Business Definition
Geography dimension representing the sales geography hierarchy used for regional performance reporting.

## Technical Mapping
- Technical Table: `dim_geography`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
| Geography Key | `geography_key` | Surrogate key that uniquely identifies a geography record. |
| Region | `region` | Broad sales region associated with the booking or sales coverage model. |
| Theater | `theater` | Intermediate geography grouping used within Cisco sales organization structures. |
| Country | `country` | Country associated with the geography record. |

## Keys
- Primary Key: `geography_key`

## Measures
- No explicit measures are modeled for this entity.

## Relationships
- [Geography to Booking Transaction](../relationships/geography-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts
- Domain: [Geography](../domains/geography.md)
- Related entities: [Booking Transaction](booking-transaction.md), [Customer](customer.md)
