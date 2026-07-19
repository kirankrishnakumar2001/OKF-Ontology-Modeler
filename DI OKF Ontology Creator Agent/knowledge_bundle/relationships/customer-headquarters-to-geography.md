---
title: Customer Headquarters to Geography
concept_type: relationship
source_entity: customer
target_entity: geography
relationship_type: inferred_semantic_association
cardinality: many-to-one-inferred
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
Many Customers may align to one Geography conceptually

## Business Description
This inferred relationship reflects the semantic alignment between customer headquarters fields and geography concepts. It is useful for contextual analysis but is not represented by a physical foreign key.

## Technical Basis
Based on `dim_customer.hq_country` and `dim_customer.hq_region` semantics only; no explicit foreign key is modeled.
