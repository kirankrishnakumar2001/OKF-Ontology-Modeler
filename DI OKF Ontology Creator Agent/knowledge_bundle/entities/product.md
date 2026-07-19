---
title: Product
concept_type: entity
business_domain: product
technical_mapping: dim_product
keys:
  primary_key: product_key
  business_key: product_id
---

# Product

## Business Definition
Product dimension representing Cisco products, subscriptions, and offers across portfolio and technology domains.

## Technical Mapping
- Table: `dim_product`
- Primary Key: `product_key`
- Business Key: `product_id`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Product Key | `product_key` | Surrogate key that uniquely identifies a product record in the dimension. |
| Product ID | `product_id` | Business identifier assigned to a product, SKU, or offer. |
| Product Name | `product_name` | Human-readable name of the Cisco product or offer. |
| Product Family | `product_family` | Higher-level grouping of products into common families. |
| Technology Domain | `technology_domain` | Technology area to which the product belongs. |
| Offer Type | `offer_type` | Commercial offer category for the product. |
| Business Entity | `business_entity` | Internal Cisco business unit or portfolio entity associated with the product. |

## Keys

- Primary Key: `product_key`
- Business Key: `product_id`

## Measures

This entity does not contain explicit stored measures. It contextualizes [Booking Amount USD](../measures/booking-amount-usd.md), [Annual Contract Value USD](../measures/annual-contract-value-usd.md), and [Total Contract Value USD](../measures/total-contract-value-usd.md).

## Relationships

- [Product to Booking Transaction](../relationships/product-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts

- [Product Domain](../domains/product.md)
- [Booking Transaction](booking-transaction.md)
- [Contract](contract.md)
