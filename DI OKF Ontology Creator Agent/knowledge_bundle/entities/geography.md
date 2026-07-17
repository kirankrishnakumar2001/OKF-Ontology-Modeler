---
title: Geography
concept_type: entity
technical_mapping: dim_geography
domain: ../domains/geography.md
relationships:
  - ../relationships/geography-to-booking-transaction.md
  - ../relationships/customer-headquarters-to-geography.md
---

# Geography

## Business Definition

Geography entity representing sales geography hierarchy across region, theater, and country for reporting and rollups.

## Technical Mapping

- Table: `dim_geography`
- Entity Type: Dimension
- Primary Key: `geography_key`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Geography Key | `geography_key` | Surrogate key uniquely identifying a geography record. |
| Region | `region` | Broad sales region associated with the record. |
| Theater | `theater` | Intermediate geography grouping used within sales structures. |
| Country | `country` | Country associated with the geography record. |

## Keys

- Primary Key: `geography_key`

## Measures

- None explicit.

## Relationships

- [Geography to Booking Transaction](../relationships/geography-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts

- Domain: [Geography](../domains/geography.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
- Related customer context: [Customer](customer.md)
