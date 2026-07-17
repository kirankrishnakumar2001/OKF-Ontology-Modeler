---
title: Date
concept_type: entity
technical_mapping: dim_date
domain: ../domains/time.md
relationships:
  - ../relationships/date-to-booking-transaction.md
---

# Date

## Business Definition

Date entity representing calendar and fiscal reporting periods for bookings analysis.

## Technical Mapping

- Table: `dim_date`
- Entity Type: Dimension
- Primary Key: `date_key`
- Business Key: `full_date`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Date Key | `date_key` | Surrogate or encoded key uniquely identifying a date record. |
| Full Date | `full_date` | Actual calendar date represented by the dimension row. |
| Month Name | `month_name` | Name of the calendar month. |
| Calendar Year | `calendar_year` | Four-digit calendar year. |
| Fiscal Year | `fiscal_year` | Cisco fiscal year associated with the date. |
| Fiscal Quarter | `fiscal_quarter` | Cisco fiscal quarter associated with the date. |
| Fiscal Period Sequence | `fiscal_period_seq` | Sequential numeric ordering of fiscal periods. |

## Keys

- Primary Key: `date_key`
- Business Key: `full_date`

## Measures

- None explicit.

## Relationships

- [Date to Booking Transaction](../relationships/date-to-booking-transaction.md)

## Related Concepts

- Domain: [Time](../domains/time.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
