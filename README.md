# 🛡️ EHR Patient Safety & HIPAA Risk Assessment

Three healthcare risk analyses using the quality and safety tools hospitals rely on: **root cause analysis**, **Failure Mode and Effects Analysis (FMEA)**, and a **HIPAA Security Rule risk assessment**.

*Coursework from HCIN 630: Health Care Law & Risk Management and HCIN 544: Advanced Health Care Information Management, MS in Health Care Informatics, University of San Diego*

---

## 1️⃣ Root Cause Analysis: *Lowe v. Cerner Corporation*

### The Case
After gallbladder surgery at Virginia Hospital Center, a 25-year-old patient's surgeon ordered **continuous pulse oximetry** in the Cerner EHR. The order was meant to start right after surgery, but the system showed a start time of **10:00 a.m. the next day**. The patient's oxygen levels weren't monitored overnight, and he suffered **hypoxic brain damage**. In 2022, the U.S. Court of Appeals for the Fourth Circuit ruled that a jury could find the EHR software had design defects, which made it a landmark case for **EHR vendor accountability**.

### Fishbone (Cause-and-Effect) Diagram

![Fishbone diagram](images/fishbone_diagram.png)

### 5 Whys
1. The patient's oxygen saturation dropped to a critical level without anyone noticing.
2. Continuous pulse oximetry wasn't running, even though the physician had ordered it.
3. The EHR changed the order's start time, which delayed it.
4. The EHR's order-scheduling logic silently changed time-sensitive orders without telling clinical staff.
5. **Root cause:** the software limitation hadn't been disclosed to hospital customers, and no verification step existed to catch the change.

### Proposed Solution: EHR Order Entry Safety Process

![Order entry safety flowchart](images/order_entry_safety_flowchart.png)

**Key recommendations:**
- A real-time **alert whenever the EHR overrides a physician's order settings**, which the physician must acknowledge
- **Individual review** of high-risk and time-sensitive orders, instead of batch approval
- **Nurse verification** that the order matches the intended care plan, with a clear escalation path
- **Vendor disclosure** of known software limitations, plus training on how the system handles orders

📄 [5 Whys analysis (PDF)](lowe-v-cerner-root-cause-analysis/Lowe_v_Cerner_5_Whys_Root_Cause_Analysis.pdf) · [Fishbone diagram (PDF)](lowe-v-cerner-root-cause-analysis/Lowe_v_Cerner_Fishbone_Diagram.pdf)

---

## 2️⃣ FMEA: EHR Drug-Allergy Alert & Override Process

A **prospective** risk analysis of how a medication-allergy safety process could fail, from admission to bedside. Each step is scored on severity and probability to get a hazard score.

| # | Process Step | Potential Failure | Hazard Score | Action |
|---|---|---|---|---|
| 1 | Allergy entry at admission | Allergy missing or entered incorrectly | **12** (Catastrophic × Occasional) | Eliminate |
| 2 | CDS allergy alert at prescribing | Alert fails to fire or is suppressed | **8** (Catastrophic × Uncommon) | Eliminate |
| 3 | Clinician override of alert | Override without clinical justification | **12** (Catastrophic × Occasional) | Eliminate |
| 4 | Pharmacist dispensing review | Allergy conflict not caught before dispensing | **9** (Major × Occasional) | Control |
| 5 | Nurse administration and patient ID | Allergen given without bedside check | **8** (Catastrophic × Uncommon) | Control |

**Highlights of the mitigation plan:** a required allergy field at admission, hard-stop alerts for the most severe interactions, a written justification for every override, a red allergy banner on the pharmacist's screen that can't be hidden, barcode-scan allergy alerts at the bedside, and regular simulation training.

📄 [Full FMEA (PDF)](fmea/FMEA_EHR_Drug_Allergy_Alert_Process.pdf)

---

## 3️⃣ HIPAA Privacy & Security Risk Assessment

A HIPAA Security Rule desk audit of a case-study outpatient clinic using the **CMS/ONC Security Risk Assessment Tool**. It found **17 risks** (6 High, 10 Medium, 1 Low) across administrative, technical, and physical safeguards, each with a mitigation plan.

**Top high-impact findings:** no role-based access limits, no periodic access reviews, unmanaged devices reaching the cloud EHR, and no media sanitization procedure.

📄 [Full findings and recommendations](hipaa-security-risk-assessment/HIPAA_Security_Risk_Assessment.md)

---

## 🛠️ Skills Demonstrated
Root Cause Analysis · 5 Whys · Fishbone (Ishikawa) Diagrams · Process Flowcharting · FMEA · Patient Safety · Clinical Decision Support Governance · HIPAA Security Rule · CMS SRA Tool · NIST CSF · Risk Mitigation Planning

---

👩‍💻 **Prerna Sinha** · [LinkedIn](https://www.linkedin.com/in/prerna-sinha-health-informatics/) · [ePortfolio](https://sites.google.com/view/prernasinha/home)
