---
title: Semantic Summary
subject_area: Cisco Sales Bookings and Revenue Analytics
status: validated-with-warnings
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
| OSI Semantic Model readability | Pass | Source semantic model content was readable from `DI OSI Semantic Creator Agent Output.txt`. |
| Business Process document readability | Pass | `Cisco_Bookings_Data_Model_and_Process.docx` was readable. |
| Required semantic sections present | Pass | Domains, entities, relationships, measures, glossary mapping, metrics, and validation were present. |
| Duplicate entities | Pass | No duplicate entities detected. |
| Duplicate domains | Pass | No duplicate domains detected. |
| Missing relationships | Warning | Explicit FK relationships are complete; two additional semantic associations are inferred rather than physically modeled. |
| Data-backed validation | Warning | Source tables were reported as empty, limiting empirical validation of domains, values, and metrics. |

## Extracted Business Domains

- [Sales Bookings](domains/sales-bookings.md)
- [Customer](domains/customer.md)
- [Product](domains/product.md)
- [Partner / Channel](domains/partner-channel.md)
- [Geography](domains/geography.md)
- [Sales Organization](domains/sales-organization.md)
- [Contract](domains/contract.md)
- [Time](domains/time.md)

## Extracted Business Entities

- [Booking Transaction](entities/booking-transaction.md)
- [Customer](entities/customer.md)
- [Product](entities/product.md)
- [Partner](entities/partner.md)
- [Geography](entities/geography.md)
- [Sales Representative](entities/sales-representative.md)
- [Contract](entities/contract.md)
- [Date](entities/date.md)

## Extracted Relationships

- [Date to Booking Transaction](relationships/date-to-booking-transaction.md)
- [Customer to Booking Transaction](relationships/customer-to-booking-transaction.md)
- [Product to Booking Transaction](relationships/product-to-booking-transaction.md)
- [Partner to Booking Transaction](relationships/partner-to-booking-transaction.md)
- [Geography to Booking Transaction](relationships/geography-to-booking-transaction.md)
- [Sales Representative to Booking Transaction](relationships/sales-representative-to-booking-transaction.md)
- [Contract to Booking Transaction](relationships/contract-to-booking-transaction.md)
- [Customer Headquarters to Geography](relationships/customer-headquarters-to-geography.md)
- [Product to Contract Applicability](relationships/product-to-contract-applicability.md)

## Extracted Measures

- [Quantity Sold](measures/quantity-sold.md)
- [Unit List Price USD](measures/unit-list-price-usd.md)
- [Discount Percentage](measures/discount-percentage.md)
- [Booking Amount USD](measures/booking-amount-usd.md)
- [Annual Contract Value USD](measures/annual-contract-value-usd.md)
- [Total Contract Value USD](measures/total-contract-value-usd.md)

## Knowledge Extraction Notes

The business process document enriches the semantic model by clarifying:

- quote-to-booking process boundaries
- booking recognition timing
- distinction between bookings, billings, and revenue
- role ownership across Sales, Deal Desk, Revenue Operations, Channel/Partner Org, Customer Experience, and Finance
- KPI interpretation for bookings, renewal mix, ACV, TCV, attach rate, product-family mix, and partner contribution

## Bundle Validation Summary

| Validation Check | Status | Details |
| --- | --- | --- |
| Missing concept documents | Pass | All extracted domains, entities, relationships, measures, and glossary terms were generated as concept documents. |
| Missing YAML frontmatter | Pass | All generated Markdown documents include YAML frontmatter. |
| Broken semantic links | Pass | Internal semantic links were generated consistently using relative paths. |
| Duplicate concept documents | Pass | No duplicate concept documents were generated. |
| Missing references | Warning | Some inferred concepts reference business-process semantics rather than explicit modeled foreign keys. |
