---
title: Partner to Booking Transaction
concept_type: relationship
source_entity: partner
target_entity: booking-transaction
relationship_type: dimensional_foreign_key
cardinality: one-to-many
---

# Partner to Booking Transaction

## Source Entity
- [Partner](../entities/partner.md)

## Target Entity
- [Booking Transaction](../entities/booking-transaction.md)

## Relationship Type
Dimensional foreign key

## Cardinality
One Partner to many Booking Transactions

## Business Description
Each booking transaction may be associated with a partner organization, supporting route-to-market and channel performance analysis.

## Technical Basis
`fact_bookings.partner_key -> dim_partner.partner_key`
