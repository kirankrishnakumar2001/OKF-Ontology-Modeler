---
title: Customer
concept_type: entity
technical_table_name: dim_customer
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/customer.md
related_relationships:
  - ../relationships/customer-to-booking-transaction.md
  - ../relationships/customer-headquarters-to-geography.md
---

# Customer

## Business Definition
Customer dimension representing the buying account used for segmentation, industry, and headquarters-based analysis.

## Technical Mapping
- Technical Table: `dim_customer`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
| Customer Key | `customer_key` | Surrogate key that uniquely identifies a customer record in the dimension. |
| Customer ID | `customer_id` | Business identifier assigned to a customer account. |
| Customer Name | `customer_name` | Official name of the customer account placing the order. |
| Customer Segment | `segment` | Market segment to which the customer belongs. |
| Industry | `industry` | Industry classification of the customer account. |
| Account Tier | `account_tier` | Tier or strategic ranking assigned to the customer account. |
| Headquarters Country | `hq_country` | Country where the customer headquarters is located. |
| Headquarters Region | `hq_region` | Region where the customer headquarters is located. |

## Keys
- Primary Key: `customer_key`
- Business Key: `customer_id`

## Measures
- No explicit measures are modeled for this entity.

## Relationships
- [Customer to Booking Transaction](../relationships/customer-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts
- Domain: [Customer](../domains/customer.md)
- Related entity: [Booking Transaction](booking-transaction.md)
- Related entity: [Geography](geography.md)
