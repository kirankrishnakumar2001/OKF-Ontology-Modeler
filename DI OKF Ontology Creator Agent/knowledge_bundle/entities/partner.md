---
title: Partner
concept_type: entity
technical_table_name: dim_partner
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/partner-channel.md
related_relationships:
  - ../relationships/partner-to-booking-transaction.md
---

# Partner

## Business Definition
Partner dimension representing channel organizations participating in indirect sales and route-to-market analysis.

## Technical Mapping
- Technical Table: `dim_partner`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
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
- No explicit measures are modeled for this entity.

## Relationships
- [Partner to Booking Transaction](../relationships/partner-to-booking-transaction.md)

## Related Concepts
- Domain: [Partner / Channel](../domains/partner-channel.md)
- Related entity: [Booking Transaction](booking-transaction.md)
