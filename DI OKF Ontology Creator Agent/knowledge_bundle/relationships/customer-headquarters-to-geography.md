---
title: Customer Headquarters to Geography
concept_type: relationship
source_entity: ../entities/customer.md
target_entity: ../entities/geography.md
relationship_type: inferred semantic association
cardinality: Many-to-One inferred
confidence_score: 0.55
---

# Customer Headquarters to Geography

## Source Entity

- [Customer](../entities/customer.md)

## Target Entity

- [Geography](../entities/geography.md)

## Relationship Type

Inferred semantic association

## Cardinality

Many customers may align to one geography conceptually.

## Business Description

This association is inferred from the customer attributes `hq_country` and `hq_region`. It provides contextual alignment between customer headquarters and geography reporting, but no explicit foreign key was modeled.
