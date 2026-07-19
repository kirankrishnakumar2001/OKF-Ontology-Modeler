---
title: Semantic Summary
concept_type: semantic_summary
business_subject_area: Cisco Sales Bookings and Revenue Analytics
source_documents:
  - DI OSI Semantic Creator Agent Output.txt
  - Cisco_Bookings_Data_Model_and_Process.docx
---

# Semantic Summary

## Semantic Overview

| Section | Value |
| --- | --- |
| Business Subject Area | Cisco Sales Bookings and Revenue Analytics |
| Data Domain Description | Star-schema analytical model for Cisco booking transactions at order-line grain with conformed dimensions for customer, product, partner, geography, sales representative, contract, and date. |
| Business Value Proposition | Provides a governed semantic foundation for consistent analysis of bookings, ACV, TCV, quantity, discounting, partner contribution, product mix, renewals, and fiscal performance across Cisco sales operations. |
| Business Capabilities Enabled | Booking performance reporting; customer and segment analysis; product portfolio analysis; partner and route-to-market analysis; geography reporting; sales performance management; contract and renewal analysis; fiscal period reporting; executive dashboards; semantic reuse for downstream analytics and knowledge modeling |
| Business Question 1 | What is total booking amount by fiscal year, fiscal quarter, region, and product family? |
| Business Question 2 | How do renewal bookings and ACV/TCV vary by contract type, offer type, and customer segment? |
| Business Question 3 | What is partner contribution to bookings by route to market, theater, and sales team? |

## Input Validation

| Validation Check | Status | Details |
| --- | --- | --- |
| OSI Semantic Model readability | Pass | The OSI semantic model output was readable and structurally complete. |
| Business Process document readability | Pass | `Cisco_Bookings_Data_Model_and_Process.docx` was readable. |
| Required semantic sections present | Pass | Domains, entities, relationships, measures, glossary mapping, summary, metrics, and validation were present in the source model. |
| Duplicate entities | Pass | No duplicate entities detected. |
| Duplicate domains | Pass | No duplicate domains detected. |
| Missing relationships | Pass | All seven explicit fact-to-dimension relationships are present. |
| Validation warning | Warning | Two semantic associations are inferred rather than physically modeled: Customer Headquarters to Geography and Product to Contract Applicability. |
| Validation warning | Warning | Source data rows are unavailable, so value-domain and empirical semantic validation cannot be performed. |

## Domain Summary

- [Sales Bookings](domains/sales-bookings.md)
- [Customer](domains/customer.md)
- [Product](domains/product.md)
- [Partner / Channel](domains/partner-channel.md)
- [Geography](domains/geography.md)
- [Sales Organization](domains/sales-organization.md)
- [Contract](domains/contract.md)
- [Time](domains/time.md)

## Entity Summary

- [Booking Transaction](entities/booking-transaction.md)
- [Customer](entities/customer.md)
- [Product](entities/product.md)
- [Partner](entities/partner.md)
- [Geography](entities/geography.md)
- [Sales Representative](entities/sales-representative.md)
- [Contract](entities/contract.md)
- [Date](entities/date.md)

## Relationship Summary

- [Date to Booking Transaction](relationships/date-to-booking-transaction.md)
- [Customer to Booking Transaction](relationships/customer-to-booking-transaction.md)
- [Product to Booking Transaction](relationships/product-to-booking-transaction.md)
- [Partner to Booking Transaction](relationships/partner-to-booking-transaction.md)
- [Geography to Booking Transaction](relationships/geography-to-booking-transaction.md)
- [Sales Representative to Booking Transaction](relationships/sales-representative-to-booking-transaction.md)
- [Contract to Booking Transaction](relationships/contract-to-booking-transaction.md)
- [Customer Headquarters to Geography](relationships/customer-headquarters-to-geography.md)
- [Product to Contract Applicability](relationships/product-to-contract-applicability.md)

## Measure Summary

- [Quantity Sold](measures/quantity-sold.md)
- [Unit List Price USD](measures/unit-list-price-usd.md)
- [Discount Percentage](measures/discount-percentage.md)
- [Booking Amount USD](measures/booking-amount-usd.md)
- [Annual Contract Value USD](measures/annual-contract-value-usd.md)
- [Total Contract Value USD](measures/total-contract-value-usd.md)

## Glossary Summary

See [Glossary Index](glossary/index.md) for all glossary concepts.

## Knowledge Bundle Validation

| Validation Check | Status | Details |
| --- | --- | --- |
| Missing concept documents | Pass | This bundle includes domain, entity, relationship, measure, and glossary indexes and concept documents. |
| Missing YAML frontmatter | Pass | All generated documents include YAML frontmatter. |
| Broken semantic links | Pass | All links in this bundle target generated documents. |
| Duplicate concept documents | Pass | No duplicate concept documents generated. |
| Missing references | Pass | Core semantic references are present across linked concepts. |
