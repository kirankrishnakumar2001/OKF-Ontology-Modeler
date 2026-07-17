---
title: Sales Representative to Booking Transaction
concept_type: relationship
source_entity: ../entities/sales-representative.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Sales Representative to Booking Transaction

## Source Entity

- [Sales Representative](../entities/sales-representative.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One sales representative to many booking transactions.

## Business Description

Each booking transaction is assigned to a sales representative through `fact_bookings.sales_rep_key -> dim_sales_rep.sales_rep_key`, enabling sales ownership and team analysis.
