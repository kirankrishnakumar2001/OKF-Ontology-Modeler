---
title: Date to Booking Transaction
concept_type: relationship
source_entity: ../entities/date.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Date to Booking Transaction

## Source Entity

- [Date](../entities/date.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One date to many booking transactions.

## Business Description

Each booking transaction is associated with a reporting date through `fact_bookings.date_key -> dim_date.date_key`, enabling calendar and fiscal reporting.
