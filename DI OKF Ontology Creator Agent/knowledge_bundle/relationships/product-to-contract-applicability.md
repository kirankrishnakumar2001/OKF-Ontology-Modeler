---
title: Product to Contract Applicability
concept_type: relationship
source_entity: ../entities/product.md
target_entity: ../entities/contract.md
relationship_type: inferred business association
cardinality: many-to-many conceptual
bundle: Cisco Sales Bookings and Revenue Analytics
---

# Product to Contract Applicability

## Source Entity
[Product](../entities/product.md)

## Target Entity
[Contract](../entities/contract.md)

## Relationship Type
Inferred business association

## Cardinality
Many products may relate to many contract types conceptually

## Business Description
This association is inferred from the business process, which states that support and subscription offers attach to contracts and drive contract-related analysis. It is not represented as a direct physical foreign key in the source model.
