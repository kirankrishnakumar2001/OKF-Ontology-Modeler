---
title: Partner
concept_type: entity
technical_mapping: dim_partner
domain: ../domains/partner-channel.md
relationships:
  - ../relationships/partner-to-booking-transaction.md
---

# Partner

## Business Definition

Partner organization entity representing channel participants and route-to-market context for indirect sales analysis.

## Technical Mapping

- Table: `dim_partner`
- Entity Type: Dimension
- Primary Key: `partner_key`
- Business Key: `partner_id`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Partner Key | `partner_key` | Surrogate key uniquely identifying a partner record. |
| Partner ID | `partner_id` | Business identifier assigned to a partner organization. |
| Partner Name | `partner_name` | Official name of the partner organization. |
| Partner Type | `partner_type` | Classification of partner organization. |
| Partner Tier | `partner_tier` | Tier or program level assigned to the partner. |
| Route to Market | `route_to_market` | Sales route through which the booking was transacted. |

## Keys

- Primary Key: `partner_key`
- Business Key: `partner_id`

## Measures

- None explicit.

## Relationships

- [Partner to Booking Transaction](../relationships/partner-to-booking-transaction.md)

## Related Concepts

- Domain: [Partner / Channel](../domains/partner-channel.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
