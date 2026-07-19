---
title: Cisco Bookings OKF Knowledge Bundle
concept_type: knowledge_bundle_index
subject_area: Cisco Sales Bookings and Revenue Analytics
version: 1.0
status: generated
source_documents:
  - DI OSI Semantic Creator Agent Output.txt
  - Cisco_Bookings_Data_Model_and_Process.docx
---

# Cisco Bookings OKF Knowledge Bundle

This Open Knowledge Format (OKF) knowledge bundle organizes the validated Cisco bookings semantic model into reusable domain, entity, relationship, measure, and glossary concept documents.

## Navigation

- [Semantic Summary](semantic_summary.md)
- [Metrics](metrics.md)
- [Domains](domains/index.md)
- [Entities](entities/index.md)
- [Relationships](relationships/index.md)
- [Measures](measures/index.md)
- [Glossary](glossary/index.md)

## Bundle Scope

The bundle represents a star-schema analytical model for Cisco booking transactions at order-line grain with conformed dimensions for customer, product, partner, geography, sales representative, contract, and date.

## Validation Notes

- OSI Semantic Model readability: Pass
- Business process document readability: Pass
- Duplicate entities: None detected
- Duplicate domains: None detected
- Missing explicit foreign-key relationships: None detected
- Warnings: semantic associations such as Customer Headquarters to Geography and Product to Contract Applicability are inferred and confidence-scored; row-level data validation is not possible because all tables are empty.
