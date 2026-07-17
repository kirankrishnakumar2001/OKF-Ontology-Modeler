---
title: Partner to Booking Transaction
concept_type: relationship
source_entity: ../entities/partner.md
target_entity: ../entities/booking-transaction.md
relationship_type: dimensional foreign key
cardinality: One-to-Many
confidence_score: 1.00
---

# Partner to Booking Transaction

## Source Entity

- [Partner](../entities/partner.md)

## Target Entity

- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type

Dimensional foreign key

## Cardinality

One partner to many booking transactions.

## Business Description

Each booking transaction may reference a partner through `fact_bookings.partner_key -> dim_partner.partner_key`, enabling channel, partner, and route-to-market performance analysis.
