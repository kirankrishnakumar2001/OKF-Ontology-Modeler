---
title: Metrics
bundle: Cisco Sales Bookings and Revenue Analytics
format: OKF
version: 1.0
status: generated
---

# Metrics

## Overall Metrics

| Metric | Value |
|---|---:|
| Total Tables / Entities | 8 |
| Total Attributes / Columns | 61 |
| Total Relationships | 9 |
| Total Domains | 8 |
| Total Measures | 6 |
| Total Glossary Terms | 69 |
| Mapped Terms | 69 |
| Glossary Coverage Percentage | 100.00% |

## Per-Domain Metrics

| Domain | Entity Count | Attribute Count | Measure Count | Glossary Coverage | Status |
|---|---:|---:|---:|---:|---|
| Sales Bookings | 1 | 12 | 6 | 100.00% | Structurally complete; data unavailable |
| Customer | 1 | 6 | 0 | 100.00% | Structurally complete; data unavailable |
| Product | 1 | 6 | 0 | 100.00% | Structurally complete; data unavailable |
| Partner / Channel | 1 | 5 | 0 | 100.00% | Structurally complete; data unavailable |
| Geography | 1 | 3 | 0 | 100.00% | Structurally complete; data unavailable |
| Sales Organization | 1 | 5 | 0 | 100.00% | Structurally complete; data unavailable |
| Contract | 1 | 4 | 0 | 100.00% | Structurally complete; data unavailable |
| Time | 1 | 6 | 0 | 100.00% | Structurally complete; data unavailable |

## KPI Context from Business Process
- Total Bookings: headline demand metric based on net booked value in a period.
- Net-New vs Renewal mix: driven by booking type and renewal indicator.
- ACV / TCV: key measures for subscriptions and SaaS.
- Renewal capture rate: business KPI referenced in process context, but not modeled as an explicit stored measure in the source semantic model.
- Attach rate: business KPI referenced in process context, but not modeled as an explicit stored measure in the source semantic model.
- Product-family mix and partner contribution are enabled analytically through dimension slicing.

## Generation Validation

| Validation Check | Status | Notes |
|---|---|---|
| Missing concept documents | Pass | Documents were generated for all source concepts represented in the bundle. |
| Missing YAML frontmatter | Pass | All generated markdown files include YAML frontmatter. |
| Broken semantic links | Pass | All internal links reference generated files in the bundle structure. |
| Duplicate concept documents | Pass | No duplicate concept documents generated. |
| Missing references | Partial Pass | Inferred relationships are documented with confidence notes; no explicit source references were missing for physical concepts. |
