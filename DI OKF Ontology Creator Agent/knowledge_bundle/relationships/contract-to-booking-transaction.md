---
title: Contract to Booking Transaction
concept_type: relationship
source_entity: ../entities/contract.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Contract to Booking Transaction

## Source Entity

- [Contract](../entities/contract.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One contract to many booking transactions.

## Business Description

Each booking transaction may be linked to contract context through `fact_bookings.contract_key -> dim_contract.contract_key`, enabling renewal, term, coverage, ACV, and TCV analysis.
