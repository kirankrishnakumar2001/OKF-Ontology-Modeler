---
title: Contract
concept_type: entity
technical_table_name: dim_contract
entity_type: dimension
bundle: Cisco Sales Bookings and Revenue Analytics
related_domain: ../domains/contract.md
related_relationships:
  - ../relationships/contract-to-booking-transaction.md
  - ../relationships/product-to-contract-applicability.md
---

# Contract

## Business Definition
Contract dimension representing service, support, or subscription agreement context associated with bookings.

## Technical Mapping
- Technical Table: `dim_contract`
- Entity Type: Dimension

## Attributes
| Attribute | Technical Column | Business Definition |
|---|---|---|
| Contract Key | `contract_key` | Surrogate key that uniquely identifies a contract record in the dimension. |
| Contract Type | `contract_type` | Type of commercial agreement associated with a booking, such as service, support, or subscription contract. |
| Contract Term Months | `term_months` | Number of months covered by the contract term. |
| Auto Renewal Indicator | `auto_renew_flag` | Flag indicating whether the contract is configured to renew automatically. |
| Coverage Level | `coverage_level` | Service or support level provided by the contract. |

## Keys
- Primary Key: `contract_key`

## Measures
- No explicit measures are modeled for this entity.

## Relationships
- [Contract to Booking Transaction](../relationships/contract-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts
- Domain: [Contract](../domains/contract.md)
- Related entities: [Booking Transaction](booking-transaction.md), [Product](product.md)
