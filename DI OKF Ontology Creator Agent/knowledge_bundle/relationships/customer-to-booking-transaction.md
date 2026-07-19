---
title: Customer to Booking Transaction
concept_type: relationship
source_entity: customer
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Customer to Booking Transaction

## Source Entity
- [Customer](../entities/customer.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Customer to many Booking Transactions

## Business Description
Each booking transaction belongs to a customer account, enabling analysis by customer name, segment, industry, and headquarters context.

## Technical Basis
`fact_bookings.customer_key -> dim_customer.customer_key`
