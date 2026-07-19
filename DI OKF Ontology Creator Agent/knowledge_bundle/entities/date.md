---
title: Date
concept_type: entity
business_domain: time
technical_mapping: dim_date
keys:
  primary_key: date_key
  business_key: full_date
---

# Date

## Business Definition
Date dimension representing calendar and fiscal reporting periods for bookings analysis.

## Technical Mapping
- Table: `dim_date`
- Primary Key: `date_key`
- Business Key: `full_date`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
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

This entity does not contain explicit stored measures. It contextualizes [Booking Amount USD](../measures/booking-amount-usd.md), [Annual Contract Value USD](../measures/annual-contract-value-usd.md), [Total Contract Value USD](../measures/total-contract-value-usd.md), and [Quantity Sold](../measures/quantity-sold.md).

## Relationships

- [Date to Booking Transaction](../relationships/date-to-booking-transaction.md)

## Related Concepts

- [Time Domain](../domains/time.md)
- [Booking Transaction](booking-transaction.md)
