---
title: Customer
concept_type: entity
business_domain: customer
technical_mapping: dim_customer
keys:
  primary_key: customer_key
  business_key: customer_id
---

# Customer

## Business Definition
Customer dimension representing the buying account used for segmentation, industry, and headquarters-based analysis.

## Technical Mapping
- Table: `dim_customer`
- Primary Key: `customer_key`
- Business Key: `customer_id`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
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

This entity does not contain explicit stored measures. It contextualizes measures such as [Booking Amount USD](../measures/booking-amount-usd.md) and [Annual Contract Value USD](../measures/annual-contract-value-usd.md).

## Relationships

- [Customer to Booking Transaction](../relationships/customer-to-booking-transaction.md)
- [Customer Headquarters to Geography](../relationships/customer-headquarters-to-geography.md)

## Related Concepts

- [Customer Domain](../domains/customer.md)
- [Booking Transaction](booking-transaction.md)
- [Geography](geography.md)
