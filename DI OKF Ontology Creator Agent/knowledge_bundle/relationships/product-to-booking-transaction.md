---
title: Product to Booking Transaction
concept_type: relationship
source_entity: product
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Product to Booking Transaction

## Source Entity
- [Product](../entities/product.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Product to many Booking Transactions

## Business Description
Each booking transaction references a Cisco product or offer, enabling analysis by product family, technology domain, offer type, and business entity.

## Technical Basis
`fact_bookings.product_key -> dim_product.product_key`
