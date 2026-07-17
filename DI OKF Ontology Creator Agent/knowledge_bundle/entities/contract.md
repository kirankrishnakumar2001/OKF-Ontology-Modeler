---
title: Contract
concept_type: entity
technical_mapping: dim_contract
domain: ../domains/contract.md
relationships:
  - ../relationships/contract-to-booking-transaction.md
  - ../relationships/product-to-contract-applicability.md
---

# Contract

## Business Definition

Contract entity representing service, support, or subscription agreement context associated with bookings.

## Technical Mapping

- Table: `dim_contract`
- Entity Type: Dimension
- Primary Key: `contract_key`

## Attributes

| Attribute | Technical Column | Business Meaning |
| --- | --- | --- |
| Contract Key | `contract_key` | Surrogate key uniquely identifying a contract record. |
| Contract Type | `contract_type` | Type of commercial agreement associated with a booking. |
| Contract Term Months | `term_months` | Number of months covered by the contract term. |
| Auto Renewal Indicator | `auto_renew_flag` | Flag indicating whether the contract is configured to renew automatically. |
| Coverage Level | `coverage_level` | Service or support level provided by the contract. |

## Keys

- Primary Key: `contract_key`

## Measures

- None explicit.

## Relationships

- [Contract to Booking Transaction](../relationships/contract-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts

- Domain: [Contract](../domains/contract.md)
- Related fact entity: [Booking Transaction](booking-transaction.md)
- Related product context: [Product](product.md)
