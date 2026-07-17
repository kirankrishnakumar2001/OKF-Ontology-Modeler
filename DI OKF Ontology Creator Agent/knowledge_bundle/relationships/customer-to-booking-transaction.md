---
title: Customer to Booking Transaction
concept_type: relationship
source_entity: ../entities/customer.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: one-to-many
bundle: Cisco Sales Bookings and Revenue Analytics
---

# Customer to Booking Transaction

## Source Entity
[Customer](../entities/customer.md)

## Target Entity
[Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One customer to many booking transactions

## Business Description
Each booking transaction belongs to a customer account. This relationship supports segmentation, industry, account-tier, and headquarters-based analysis of bookings.
