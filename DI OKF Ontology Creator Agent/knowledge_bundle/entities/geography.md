---
title: Geography
concept_type: entity
business_domain: geography
technical_mapping: dim_geography
keys:
  primary_key: geography_key
---

# Geography

## Business Definition
Geography dimension representing the sales geography hierarchy used for regional performance reporting.

## Technical Mapping
- Table: `dim_geography`
- Primary Key: `geography_key`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Geography Key | `geography_key` | Surrogate key that uniquely identifies a geography record. |
| Region | `region` | Broad sales region associated with the booking or sales coverage model. |
| Theater | `theater` | Intermediate geography grouping used within Cisco sales organization structures. |
| Country | `country` | Country associated with the geography record. |

## Keys

- Primary Key: `geography_key`

## Measures

This entity does not contain explicit stored measures. It contextualizes [Booking Amount USD](../measures/booking-amount-usd.md), [Quantity Sold](../measures/quantity-sold.md), and [Annual Contract Value USD](../measures/annual-contract-value-usd.md).

## Relationships

- [Geography to Booking Transaction](../relationships/geography-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts

- [Geography Domain](../domains/geography.md)
- [Booking Transaction](booking-transaction.md)
- [Customer](customer.md)
