---
title: Geography to Booking Transaction
concept_type: relationship
source_entity: ../entities/geography.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Geography to Booking Transaction

## Source Entity

- [Geography](../entities/geography.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One geography to many booking transactions.

## Business Description

Each booking transaction is associated with a sales geography through `fact_bookings.geography_key -> dim_geography.geography_key`, enabling region, theater, and country rollups.
