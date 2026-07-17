---
title: Product
concept_type: entity
technical_table_name: dim_product
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/product.md
related_relationships:
  - ../relationships/product-to-booking-transaction.md
  - ../relationships/product-to-contract-applicability.md
---

# Product

## Business Definition
Product dimension representing Cisco products, subscriptions, and offers across portfolio and technology domains.

## Technical Mapping
- Technical Table: `dim_product`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
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
- No explicit measures are modeled for this entity.

## Relationships
- [Product to Booking Transaction](../relationships/product-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts
- Domain: [Product](../domains/product.md)
- Related entity: [Booking Transaction](booking-transaction.md)
- Related entity: [Contract](contract.md)
