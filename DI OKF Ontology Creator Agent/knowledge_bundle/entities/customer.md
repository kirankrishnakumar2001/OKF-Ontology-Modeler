---
title: Customer
concept_type: entity
technical_mapping: dim_customer
domain: ../domains/customer.md
relationships:
  - ../relationships/customer-to-booking-transaction.md
  - ../relationships/customer-headquarters-to-geography.md
---

# Customer

## Business Definition

Customer account entity used for segmentation, industry, account-tier, and headquarters-based analysis of bookings.

## Technical Mapping

- Table: `dim_customer`
- Entity Type: Dimension
- Primary Key: `customer_key`
- Business Key: `customer_id`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Customer Key | `customer_key` | Surrogate key uniquely identifying a customer record. |
| Customer ID | `customer_id` | Business identifier assigned to a customer account. |
| Customer Name | `customer_name` | Official name of the customer account. |
| Customer Segment | `segment` | Market segment to which the customer belongs. |
| Industry | `industry` | Industry classification of the customer account. |
| Account Tier | `account_tier` | Tier or strategic ranking assigned to the customer account. |
| Headquarters Country | `hq_country` | Country where the customer headquarters is located. |
| Headquarters Region | `hq_region` | Region where the customer headquarters is located. |

## Keys

- Primary Key: `customer_key`
- Business Key: `customer_id`

## Measures

- None explicit.

## Relationships

- [Customer to Booking Transaction](../relationships/customer-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts

- Domain: [Customer](../domains/customer.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
- Related geography context: [Geography](geography.md)
