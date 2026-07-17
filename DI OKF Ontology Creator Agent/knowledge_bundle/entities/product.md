---
title: Product
concept_type: entity
technical_mapping: dim_product
domain: ../domains/product.md
relationships:
  - ../relationships/product-to-booking-transaction.md
  - ../relationships/product-to-contract-applicability.md
---

# Product

## Business Definition

Product or offer entity representing Cisco products, subscriptions, and commercial offers across product families and technology domains.

## Technical Mapping

- Table: `dim_product`
- Entity Type: Dimension
- Primary Key: `product_key`
- Business Key: `product_id`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Product Key | `product_key` | Surrogate key uniquely identifying a product record. |
| Product ID | `product_id` | Business identifier assigned to a product, SKU, or offer. |
| Product Name | `product_name` | Human-readable product or offer name. |
| Product Family | `product_family` | Higher-level grouping of products into families. |
| Technology Domain | `technology_domain` | Technology area to which the product belongs. |
| Offer Type | `offer_type` | Commercial offer category for the product. |
| Business Entity | `business_entity` | Internal Cisco business unit or portfolio entity associated with the product. |

## Keys

- Primary Key: `product_key`
- Business Key: `product_id`

## Measures

- None explicit.

## Relationships

- [Product to Booking Transaction](../relationships/product-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts

- Domain: [Product](../domains/product.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
- Related contract context: [Contract](contract.md)
