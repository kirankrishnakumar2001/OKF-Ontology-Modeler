---
title: Date
concept_type: entity
technical_table_name: dim_date
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/time.md
related_relationships:
  - ../relationships/date-to-booking-transaction.md
---

# Date

## Business Definition
Date dimension representing calendar and fiscal reporting periods for bookings analysis.

## Technical Mapping
- Technical Table: `dim_date`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
| Date Key | `date_key` | Surrogate or encoded key that uniquely identifies a date record. |
| Full Date | `full_date` | The actual calendar date represented by the dimension row. |
| Month Name | `month_name` | Name of the calendar month for the date. |
| Calendar Year | `calendar_year` | Four-digit calendar year of the date. |
| Fiscal Year | `fiscal_year` | Cisco fiscal year associated with the date. |
| Fiscal Quarter | `fiscal_quarter` | Cisco fiscal quarter associated with the date. |
| Fiscal Period Sequence | `fiscal_period_seq` | Sequential numeric ordering of fiscal periods. |

## Keys
- Primary Key: `date_key`
- Business Key: `full_date`

## Measures
- No explicit measures are modeled for this entity.

## Relationships
- [Date to Booking Transaction](../relationships/date-to-booking-transaction.md)

## Related Concepts
- Domain: [Time](../domains/time.md)
- Related entity: [Booking Transaction](booking-transaction.md)
