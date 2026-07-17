---
title: OKF Knowledge Bundle Index
bundle: Cisco Bookings OKF Knowledge Bundle
version: 1.0
status: validated-with-warnings
subject_area: Cisco Sales Bookings and Revenue Analytics
---

# Cisco Bookings OKF Knowledge Bundle

This Open Knowledge Format (OKF) knowledge bundle represents the validated semantic knowledge derived from the Cisco bookings semantic model and supporting business process documentation.

## Navigation

- [Semantic Summary](semantic_summary.md)
- [Metrics](metrics.md)
- [Domains](domains/index.md)
- [Entities](entities/index.md)
- [Relationships](relationships/index.md)
- [Measures](measures/index.md)
- [Glossary](glossary/index.md)

## Bundle Scope

- Subject Area: Cisco Sales Bookings and Revenue Analytics
- Core Grain: booking transaction at order-line grain
- Modeling Style: star schema semantic model
- Primary Fact Concept: [Booking Transaction](entities/booking-transaction.md)

## Validation Warnings

- All source tables were reported as empty, so value-domain and data-backed validation are limited.
- Some business semantics remain inferred for `booking_type`, `is_renewal`, `auto_renew_flag`, and contextual associations.
- Inferred semantic associations are preserved and clearly labeled separately from explicit foreign key relationships.

## Core Concepts

### Domains

- [Sales Bookings](domains/sales-bookings.md)
- [Customer](domains/customer.md)
- [Product](domains/product.md)
- [Partner / Channel](domains/partner-channel.md)
- [Geography](domains/geography.md)
- [Sales Organization](domains/sales-organization.md)
- [Contract](domains/contract.md)
- [Time](domains/time.md)

### Primary Measures

- [Booking Amount USD](measures/booking-amount-usd.md)
- [Annual Contract Value USD](measures/annual-contract-value-usd.md)
- [Total Contract Value USD](measures/total-contract-value-usd.md)
- [Quantity Sold](measures/quantity-sold.md)
- [Unit List Price USD](measures/unit-list-price-usd.md)
- [Discount Percentage](measures/discount-percentage.md)

### Key Entities

- [Booking Transaction](entities/booking-transaction.md)
- [Customer](entities/customer.md)
- [Product](entities/product.md)
- [Partner](entities/partner.md)
- [Geography](entities/geography.md)
- [Sales Representative](entities/sales-representative.md)
- [Contract](entities/contract.md)
- [Date](entities/date.md)
