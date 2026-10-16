# 🔒 HIPAA Privacy & Security Risk Assessment: Waverly Family Health Services

*HCIN 544: Advanced Health Care Information Management, MS in Health Care Informatics, University of San Diego*

## Overview
A HIPAA Security Rule risk assessment of **Waverly Family Health Services**, a case-study outpatient practice that uses a cloud-based EHR. The assessment was a **desk audit** using the **CMS/ONC Security Risk Assessment (SRA) Tool**. Desk-audit interview data was mapped to HIPAA administrative, technical, and physical safeguards, and each gap was rated High, Medium, or Low with a mitigation plan.

## Deliverables Produced
1. **Completed CMS SRA Tool**: safeguard-by-safeguard responses with HIPAA and NIST CSF references
2. **Privacy & Security Risk Assessment Report**: scope, ePHI inventory, business associates, role-based access review, risk ratings, and mitigation plan
3. **Information Security Policy**: a full organizational policy covering access control, passwords, encryption, malicious code, physical security, remote access, and incident response
4. **Security Governance Team proposal**: an interdisciplinary committee spanning clinical, IT, compliance, HR, and finance

---

## Findings Summary

**17 risks identified: 6 High · 10 Medium · 1 Low**

### 🔴 High-Impact Risks
| Safeguard | Risk | Mitigation |
|---|---|---|
| Technical | ePHI access not limited by role ("no limit to access") | Role-based access controls based on the **minimum-necessary** standard |
| Technical | No periodic review confirming user access is still appropriate | Scheduled access reviews tied to job role |
| Technical | Personal or unmanaged devices can reach the cloud EHR | **Mobile device management (MDM)** with device registration and approval |
| Physical | No procedure for sanitizing devices and media before disposal or reuse | Media sanitization procedure aligned with **NIST SP 800-88** |
| Physical | No access validation for personnel on critical systems | Stricter validation and logging for IT, network, and developer access |
| Administrative | Contingency plan doesn't document which systems and ePHI are most critical | Formal system and data prioritization in the contingency plan |

### 🟡 Medium-Impact Risks
- No documented workforce background screening
- Sanction policy enforcement not documented
- Security training missing some password-security elements
- Incomplete login-attempt monitoring procedures
- No documented criteria for alternatives when encryption isn't used
- Encryption incomplete across devices, cloud services, and data in transit
- No integrity controls verifying ePHI hasn't been altered or destroyed
- Third-party facility access not validated by role
- No process to end vendor access when a contract or BAA ends
- Software testing environments not separated from production

### 🟢 Low-Impact Risk
- No defined process for ending emergency procedures after an incident

---

## Top Recommendations
1. Put **role-based access control** in place with periodic access reviews
2. Complete **encryption** coverage and enforce **mobile device management**
3. Formalize **media sanitization**, **contingency planning**, and **vendor offboarding**
4. Strengthen workforce **screening, sanctions, and security training**

## Skills Demonstrated
HIPAA Security Rule · CMS/ONC SRA Tool · NIST Cybersecurity Framework · Risk Rating & Mitigation Planning · Security Policy Writing · Business Associate Agreements · Security Governance
