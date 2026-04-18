# SAP Capstone Project — Order-to-Cash (O2C): Complete Sales Cycle

> **KIIT University | B.Tech CSE | April 2026**

---

## Student Details

| Field | Details |
|---|---|
| **Name** | Priyanshu Sekhar Bhuyan |
| **Roll Number** | 2305148 |
| **Program** | B.Tech — Computer Science & Engineering (2023 - 2027) |
| **Course** | Introducing SAP Business Data Cloud |
| **Institution** | Kalinga Institute of Industrial Technology (KIIT), Bhubaneswar — 751024 |
| **Submission Date** | April 21, 2026 |

---

## Project Overview

This capstone project presents a complete, India-specific simulation of the **SAP SD Order-to-Cash (O2C)** process for **Nexus DistribuTech Pvt Ltd** — a B2B industrial automation distributor based in Bhubaneswar, Odisha. The project covers the full revenue lifecycle from customer inquiry to payment clearance, with automated SAP FI accounting and real-time analytics via SAP Business Data Cloud (BDC).

---

## SAP Modules & Technology Stack

| Layer | Technology |
|---|---|
| Transactional ERP | SAP S/4HANA Cloud (Public Edition) |
| Sales & Distribution | SAP SD — VA01 / VL01N / VF01 |
| Financial Accounting | SAP FI — F-28, VKOA, FD32 |
| Data Integration | CDS Views + OData V4 APIs |
| Analytics Platform | SAP Business Data Cloud (BDC) |
| Predictive Analytics | SAP Analytics Cloud — Smart Predict |
| Process Automation | SAP Build Process Automation |
| GST Compliance | SAP GST India Localisation |

---

## The 7-Stage O2C Cycle

| Stage | T-Code | Document | Key Action |
|---|---|---|---|
| 1. Pre-Sales Inquiry | VA11 | Inquiry (IN) | Requirement captured, no commitment |
| 2. Quotation | VA21 | Quotation (QT) | Priced quote, 20-day validity |
| 3. Sales Order | VA01 | Sales Order (OR) | ATP + credit check + pricing auto-run |
| 4. Outbound Delivery | VL01N | Delivery (LF) | Picking list, batch assignment |
| 5. Post Goods Issue | VL02N | Material Doc (WA) | Stock reduced, COGS posted to FI |
| 6. Billing / Invoice | VF01 | Invoice (F2) | AR + Revenue + GST auto-posted |
| 7. Payment Clearance | F-28 | Payment Doc (DZ) | Bank entry, AR cleared, DSO stops |

---

## Key KPI Results (90 Days Post Go-Live)

| KPI | Pre-SAP Baseline | Target | Achieved | Status |
|---|---|---|---|---|
| Order Processing Time | 5.3 days | ≤ 1 day | 0.7 days | ✅ Met |
| Invoice Error Rate | 9.8% | < 0.8% | 0.5% | ✅ Met |
| Days Sales Outstanding | 48.2 days | ≤ 38 days | 34.6 days | ✅ Met |
| On-Time Delivery Rate | 74.3% | ≥ 93% | 94.8% | ✅ Met |
| Credit Block Rate | ~6.2% | < 2.5% | 1.9% | ✅ Met |
| Gross Profit Margin | ~24.1% | ≥ 29% | 31.4% | ✅ Met |

---

## Unique Capabilities

- **Order Health Score (OHS):** Composite 0–100 index per open Sales Order — weights delivery delay risk (40%), credit exposure (35%), and ATP buffer (25%)
- **Predictive DSO Engine:** SAP Analytics Cloud regression model trained on 18 months of BSAD data — forecasts per-customer DSO with ±3-day accuracy
- **Automated Billing Block Resolution:** SAP Build Process Automation routes pricing-discrepancy blocks to the responsible account manager with a pre-filled checklist — resolution time cut from 4.1 hours to 38 minutes
- **Cross-Document Drill-Through:** Single BDC canvas linking SO → Delivery → Invoice → Payment, enabling revenue traceability in under 3 clicks

---

## Project Report

📄 **[Priyanshu_Bhuyan_O2C_Capstone_Report.pdf](./Priyanshu_Bhuyan_O2C_Capstone_Report.pdf)**

The 5-page report covers:
- Problem Statement & Organisational Context
- Complete 7-Stage O2C Process Design with sample transaction walkthrough
- SAP FI Automatic Journal Entries & Pricing Configuration
- SAP Business Data Cloud Analytics Layer & KPI Dashboard
- Unique Points, Future Roadmap & Conclusion

---

## References

1. SAP SE. *SAP SD (Sales & Distribution) Official Documentation.* help.sap.com
2. SAP SE. *SAP Business Data Cloud — Product Overview.* sap.com/products/business-data-cloud
3. SAP Learning Hub. *Introducing SAP Business Data Cloud.* KIIT SAP Training Programme, 2026.
4. SAP SE. *Credit Management in SAP S/4HANA.* SAP Help Portal, 2024.
5. KIIT SAP Project Guidance Document — Shared by Course Trainer, April 2026.
6. GST India Official Portal. *e-Invoice IRN Generation Guide.* gst.gov.in
7. Chopra, S. & Meindl, P. *Supply Chain Management: Strategy, Planning & Operation.* 7th ed. Pearson, 2022.

---

*Submitted as part of the SAP Capstone Project — KIIT University, Bhubaneswar | April 2026*
