---
title: Contract to Booking Transaction
concept_type: relationship
source_entity: contract
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Contract to Booking Transaction

## Source Entity
- [Contract](../entities/contract.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Contract to many Booking Transactions

## Business Description
Each booking transaction may be linked to contract context, enabling analysis of term, coverage, ACV, TCV, and renewal behavior.

## Technical Basis
`fact_bookings.contract_key -> dim_contract.contract_key`
