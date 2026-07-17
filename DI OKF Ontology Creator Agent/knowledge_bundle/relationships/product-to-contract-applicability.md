---
title: Product to Contract Applicability
concept_type: relationship
source_entity: ../entities/product.md
target_entity: ../entities/contract.md
relationship_type: inferred business association
cardinality: Many-to-Many conceptual
confidence_score: 0.52
---

# Product to Contract Applicability

## Source Entity

- [Product](../entities/product.md)

## Target Entity

- [Contract](../entities/contract.md)

## Relationship Type

Inferred business association

## Cardinality

Many products may relate to many contract types conceptually.

## Business Description

This association is inferred from the business process stating that support and subscription offers attach to contracts. It is preserved as semantic context, not as an explicit physical key-based relationship.
