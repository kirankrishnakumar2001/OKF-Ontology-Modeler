---
title: Sales Representative to Booking Transaction
concept_type: relationship
source_entity: sales-representative
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Sales Representative to Booking Transaction

## Source Entity
- [Sales Representative](../entities/sales-representative.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Sales Representative to many Booking Transactions

## Business Description
Each booking transaction is owned by a sales representative, supporting analysis by rep, role, team, and covered segment.

## Technical Basis
`fact_bookings.sales_rep_key -> dim_sales_rep.sales_rep_key`
