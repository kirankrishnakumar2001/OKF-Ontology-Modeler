---
title: Date to Booking Transaction
concept_type: relationship
source_entity: ../entities/date.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: one-to-many
bundle: Cisco Sales Bookings and Revenue Analytics
---

# Date to Booking Transaction

## Source Entity
[Date](../entities/date.md)

## Target Entity
[Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One date to many booking transactions

## Business Description
Each booking transaction is associated with a reporting date through the date key. This relationship enables calendar and fiscal rollup analysis, including reporting by fiscal year and fiscal quarter.
