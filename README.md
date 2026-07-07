# Veltrix Pay — Information Security Policy Suite

**Author:** John C. Ilogbene   
**Framework:** NIST SP 800-53 Rev. 5 | NIST Risk Management Framework (RMF) | PCI DSS v4.0  
**Organisation (fictional):** Veltrix Pay — Nigerian digital payments / fintech platform  
**Version:** 1.0

---

## Overview

This repository contains a complete suite of 20 information security policies developed for **Veltrix Pay**, a fictionalised Nigerian fintech company offering digital payments, merchant settlement, and card processing services.

Each policy is written for a real-world payments business context — referencing the payment switch, transaction ledger, settlement engine, cardholder data environment (CDE), KYC/AML obligations, and relationships with banks and card networks — to demonstrate applied GRC analyst competency beyond generic templates.

> **Disclaimer:** Veltrix Pay is a fictional company. All names, personnel, and configurations referenced are for portfolio demonstration purposes only and do not represent any real organisation's operational policies.

---

## Policy Index

| Policy | NIST 800-53 Family | File |
|---|---|---|
| Access Control Policy | AC | `Access_Control_Policy.md` |
| Audit & Accountability Policy | AU | `Audit_Accountability_Policy.md` |
| Awareness & Training Policy | AT | `Awareness_Training_Policy.md` |
| Configuration Management Policy | CM | `Configuration_Management_Policy.md` |
| Contingency Planning Policy | CP | `Contingency_Planning_Policy.md` |
| Identification & Authentication Policy | IA | `Identification_Authentication_Policy.md` |
| Incident Response Policy | IR | `Incident_Response_Policy.md` |
| Media Protection Policy | MP | `Media_Protection_Policy.md` |
| Personnel Security Policy | PS | `Personnel_Security_Policy.md` |
| Physical & Environmental Protection Policy | PE | `Physical_Environmental_Protection_Policy.md` |
| Planning Policy | PL | `Planning_Policy.md` |
| Privacy & PII Processing Policy | PT | `Privacy_PII_Processing_Policy.md` |
| Program Management Policy | PM | `Program_Management_Policy.md` |
| Risk Assessment Policy | RA | `Risk_Assessment_Policy.md` |
| Security Assessment & Authorization Policy | CA | `Security_Assessment_Authorization_Policy.md` |
| Supply Chain Risk Management Policy | SR | `Supply_Chain_Risk_Management_Policy.md` |
| System & Communications Protection Policy | SC | `System_Communications_Protection_Policy.md` |
| System & Information Integrity Policy | SI | `System_Information_Integrity_Policy.md` |
| System & Services Acquisition Policy | SA | `System_Services_Acquisition_Policy.md` |
| System Maintenance Policy | MA | `System_Maintenance_Policy.md` |

---

## What Makes This Suite Industry-Specific

Unlike generic NIST policy templates, every policy in this suite is tailored to a **payments/fintech operating context**:

- **PCI DSS v4.0** requirements layered alongside NIST SP 800-53 controls throughout (cardholder data environment scoping, HSM key management, quarterly vulnerability scans, annual penetration testing)
- **CBN (Central Bank of Nigeria)** regulatory references — fit-and-proper screening, payment service provider outsourcing rules, business continuity expectations
- **NDPA 2023 (Nigeria Data Protection Act)** breach notification timelines (72-hour NITDA reporting)
- **KYC/AML** retention requirements (5-year minimum per CBN)
- Payment-specific system references: payment switch, transaction ledger, settlement engine, merchant API gateway, fraud detection/transaction monitoring
- Segregation of duties specific to financial operations (transaction initiation vs. approval vs. reconciliation)

---

## Suggested GitHub Repository Structure

```
Veltrix-Pay-Policy-Suite/
├── README.md
└── Policies/
    ├── Access_Control_Policy.md
    ├── Audit_Accountability_Policy.md
    ├── Awareness_Training_Policy.md
    ├── Configuration_Management_Policy.md
    ├── Contingency_Planning_Policy.md
    ├── Identification_Authentication_Policy.md
    ├── Incident_Response_Policy.md
    ├── Media_Protection_Policy.md
    ├── Personnel_Security_Policy.md
    ├── Physical_Environmental_Protection_Policy.md
    ├── Planning_Policy.md
    ├── Privacy_PII_Processing_Policy.md
    ├── Program_Management_Policy.md
    ├── Risk_Assessment_Policy.md
    ├── Security_Assessment_Authorization_Policy.md
    ├── Supply_Chain_Risk_Management_Policy.md
    ├── System_Communications_Protection_Policy.md
    ├── System_Information_Integrity_Policy.md
    ├── System_Services_Acquisition_Policy.md
    └── System_Maintenance_Policy.md
```

---

## Recommended GitHub Repository Tags

```
nist-800-53  fintech-security  payments  pci-dss  grc
information-security  security-policy  compliance
risk-management  cybersecurity  governance  nigeria-fintech
```

---

## Author

**John C. Ilogbene**  
