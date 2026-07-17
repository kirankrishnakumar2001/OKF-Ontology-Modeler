---
title: Customer to Booking Transaction
concept_type: relationship
source_entity: ../entities/customer.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Customer to Booking Transaction

## Source Entity

- [Customer](../entities/customer.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One customer to many booking transactions.

## Business Description

Each booking transaction is linked to a customer account through `fact_bookings.customer_key -> dim_customer.customer_key`, enabling account and segment-based bookings analysis.
