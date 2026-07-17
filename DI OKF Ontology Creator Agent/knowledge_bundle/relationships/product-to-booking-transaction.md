---
title: Product to Booking Transaction
concept_type: relationship
source_entity: ../entities/product.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Product to Booking Transaction

## Source Entity

- [Product](../entities/product.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One product to many booking transactions.

## Business Description

Each booking transaction references a product or offer through `fact_bookings.product_key -> dim_product.product_key`, enabling product-family, offer-type, and technology-domain analysis.
