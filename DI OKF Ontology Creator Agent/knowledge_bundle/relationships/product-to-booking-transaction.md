---
title: Product to Booking Transaction
concept_type: relationship
source_entity: ../entities/product.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: one-to-many
bundle: Cisco Sales Bookings and Revenue Analytics
---

# Product to Booking Transaction

## Source Entity
[Product](../entities/product.md)

## Target Entity
[Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One product to many booking transactions

## Business Description
Each booking transaction references a sold product or offer. This relationship enables product family, technology domain, offer type, and business entity analysis.
