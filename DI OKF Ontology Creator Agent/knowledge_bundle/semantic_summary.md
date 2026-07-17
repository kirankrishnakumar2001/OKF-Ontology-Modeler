---
title: Semantic Summary
bundle: Cisco Sales Bookings and Revenue Analytics
format: OKF
version: 1.0
status: generated
---

# Semantic Summary

## Business Subject Area
Cisco Sales Bookings and Revenue Analytics

## Data Domain Description
Star-schema analytical model for Cisco booking transactions at order-line grain with conformed dimensions for customer, product, partner, geography, sales representative, contract, and date.

## Business Value Proposition
Provides a governed semantic foundation for consistent analysis of bookings, ACV, TCV, quantity, discounting, partner contribution, product mix, renewals, and fiscal performance across Cisco sales operations.

## Business Capabilities Enabled
- Booking performance reporting
- Customer and segment analysis
- Product portfolio analysis
- Partner and route-to-market analysis
- Geography reporting
- Sales performance management
- Contract and renewal analysis
- Fiscal period reporting
- Executive dashboards
- Semantic reuse for downstream analytics and knowledge modeling

## Core Business Questions
1. What is total booking amount by fiscal year, fiscal quarter, region, and product family?
2. How do renewal bookings and ACV/TCV vary by contract type, offer type, and customer segment?
3. What is partner contribution to bookings by route to market, theater, and sales team?

## Input Validation

| Check | Status | Notes |
|---|---|---|
| OSI Semantic Model readability | Pass | Source text file was readable. |
| Business Process document readability | Pass | Source document content was readable. |
| Required semantic sections present | Pass | Domains, entities, relationships, measures, and glossary mapping were present. |
| Duplicate entities | Pass | No duplicates identified in source model. |
| Duplicate domains | Pass | No duplicates identified in source model. |
| Missing relationships | Partial Pass | Explicit fact-to-dimension relationships are complete; two additional semantic associations are inferred only. |

## Domains in Scope
- [Sales Bookings](domains/sales-bookings.md)
- [Customer](domains/customer.md)
- [Product](domains/product.md)
- [Partner / Channel](domains/partner-channel.md)
- [Geography](domains/geography.md)
- [Sales Organization](domains/sales-organization.md)
- [Contract](domains/contract.md)
- [Time](domains/time.md)

## Entity Inventory
- [Booking Transaction](entities/booking-transaction.md)
- [Customer](entities/customer.md)
- [Product](entities/product.md)
- [Partner](entities/partner.md)
- [Geography](entities/geography.md)
- [Sales Representative](entities/sales-representative.md)
- [Contract](entities/contract.md)
- [Date](entities/date.md)

## Measure Inventory
- [Quantity Sold](measures/quantity-sold.md)
- [Unit List Price USD](measures/unit-list-price-usd.md)
- [Discount Percentage](measures/discount-percentage.md)
- [Booking Amount USD](measures/booking-amount-usd.md)
- [Annual Contract Value USD](measures/annual-contract-value-usd.md)
- [Total Contract Value USD](measures/total-contract-value-usd.md)

## Relationship Inventory
- [Date to Booking Transaction](relationships/date-to-booking-transaction.md)
- [Customer to Booking Transaction](relationships/customer-to-booking-transaction.md)
- [Product to Booking Transaction](relationships/product-to-booking-transaction.md)
- [Partner to Booking Transaction](relationships/partner-to-booking-transaction.md)
- [Geography to Booking Transaction](relationships/geography-to-booking-transaction.md)
- [Sales Representative to Booking Transaction](relationships/sales-representative-to-booking-transaction.md)
- [Contract to Booking Transaction](relationships/contract-to-booking-transaction.md)
- [Customer Headquarters to Geography](relationships/customer-headquarters-to-geography.md)
- [Product to Contract Applicability](relationships/product-to-contract-applicability.md)

## Enrichment from Business Process
The business process confirms that quote-to-booking begins with qualified opportunity handling and ends when a valid customer order is accepted and recognized as a booking. The process also establishes that bookings are distinct from billings and revenue, are additive at order-line grain, and that ACV/TCV are especially relevant for subscription and SaaS offers. Partner routing, contract creation, entitlement establishment, and renewal lifecycle management provide additional business context for the semantic relationships represented in this bundle.

## Validation Warnings
- All tables were reported with zero rows in the source semantic model, so empirical validation of value domains and measure behavior is not possible.
- Terms such as booking type, renewal indicator, business entity, and auto renewal indicator include inferred semantics with lower confidence than explicit key-based structures.
