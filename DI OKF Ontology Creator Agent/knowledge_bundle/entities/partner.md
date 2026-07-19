---
title: Partner
concept_type: entity
business_domain: partner-channel
technical_mapping: dim_partner
keys:
  primary_key: partner_key
  business_key: partner_id
---

# Partner

## Business Definition
Partner dimension representing channel organizations participating in indirect sales and route-to-market analysis.

## Technical Mapping
- Table: `dim_partner`
- Primary Key: `partner_key`
- Business Key: `partner_id`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Partner Key | `partner_key` | Surrogate key that uniquely identifies a partner record in the dimension. |
| Partner ID | `partner_id` | Business identifier assigned to a partner organization. |
| Partner Name | `partner_name` | Official name of the partner organization involved in the sale. |
| Partner Type | `partner_type` | Classification of partner organization. |
| Partner Tier | `partner_tier` | Tier or program level assigned to the partner. |
| Route to Market | `route_to_market` | Sales route through which the booking was transacted. |

## Keys

- Primary Key: `partner_key`
- Business Key: `partner_id`

## Measures

This entity does not contain explicit stored measures. It contextualizes [Booking Amount USD](../measures/booking-amount-usd.md), [Quantity Sold](../measures/quantity-sold.md), and [Discount Percentage](../measures/discount-percentage.md).

## Relationships

- [Partner to Booking Transaction](../relationships/partner-to-booking-transaction.md)

## Related Concepts

- [Partner / Channel Domain](../domains/partner-channel.md)
- [Booking Transaction](booking-transaction.md)
