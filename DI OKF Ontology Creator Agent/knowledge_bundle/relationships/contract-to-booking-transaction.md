---
title: Contract to Booking Transaction
concept_type: relationship
source_entity: ../entities/contract.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: one-to-many
bundle: Cisco Sales Bookings and Revenue Analytics
---

# Contract to Booking Transaction

## Source Entity
[Contract](../entities/contract.md)

## Target Entity
[Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One contract to many booking transactions

## Business Description
Each booking transaction may reference contract context such as agreement type, term, coverage level, and renewal settings. This relationship supports ACV, TCV, and renewal-oriented analysis.
