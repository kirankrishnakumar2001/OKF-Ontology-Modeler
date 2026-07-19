---
title: Product to Contract Applicability
concept_type: relationship
source_entity: product
target_entity: contract
relationship_type: inferred_business_association
cardinality: many-to-many-conceptual
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
Many Products may relate to many Contract concepts conceptually

## Business Description
This inferred relationship captures the business-process statement that support and subscription offers attach to contract context, even though no direct physical relationship is modeled.

## Technical Basis
Supported by the business process text on service, support, subscription, ACV, and TCV context; no direct foreign key is present.
