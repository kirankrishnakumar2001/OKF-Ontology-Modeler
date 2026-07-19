---
title: Contract
concept_type: entity
business_domain: contract
technical_mapping: dim_contract
keys:
  primary_key: contract_key
---

# Contract

## Business Definition
Contract dimension representing service, support, or subscription agreement context associated with bookings.

## Technical Mapping
- Table: `dim_contract`
- Primary Key: `contract_key`

## Attributes

| Attribute | Technical Column | Definition |
| --- | --- | --- |
| Contract Key | `contract_key` | Surrogate key that uniquely identifies a contract record in the dimension. |
| Contract Type | `contract_type` | Type of commercial agreement associated with a booking, such as service, support, or subscription contract. |
| Contract Term Months | `term_months` | Number of months covered by the contract term. |
| Auto Renewal Indicator | `auto_renew_flag` | Flag indicating whether the contract is configured to renew automatically. |
| Coverage Level | `coverage_level` | Service or support level provided by the contract. |

## Keys

- Primary Key: `contract_key`

## Measures

This entity does not contain explicit stored measures. It contextualizes [Annual Contract Value USD](../measures/annual-contract-value-usd.md), [Total Contract Value USD](../measures/total-contract-value-usd.md), and [Booking Amount USD](../measures/booking-amount-usd.md).

## Relationships

- [Contract to Booking Transaction](../relationships/contract-to-booking-transaction.md)
- [Product to Contract Applicability](../relationships/product-to-contract-applicability.md)

## Related Concepts

- [Contract Domain](../domains/contract.md)
- [Booking Transaction](booking-transaction.md)
- [Product](product.md)
