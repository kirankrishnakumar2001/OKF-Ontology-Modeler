---
title: Date to Booking Transaction
concept_type: relationship
source_entity: date
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Date to Booking Transaction

## Source Entity
- [Date](../entities/date.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Date to many Booking Transactions

## Business Description
Each booking transaction occurs on a reporting date. This relationship supports calendar and fiscal slicing of the governed bookings measures.

## Technical Basis
`fact_bookings.date_key -> dim_date.date_key`
