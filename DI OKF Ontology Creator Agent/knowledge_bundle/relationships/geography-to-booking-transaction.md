---
title: Geography to Booking Transaction
concept_type: relationship
source_entity: geography
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Geography to Booking Transaction

## Source Entity
- [Geography](../entities/geography.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Geography to many Booking Transactions

## Business Description
Each booking transaction is assigned to a sales geography, supporting regional, theater, and country reporting.

## Technical Basis
`fact_bookings.geography_key -> dim_geography.geography_key`
