# AIGAP Evidence Artifact: PRIV-01
## Data Minimisation Statement
### MediScan AI — Clinical Diagnostic Imaging Assistant

---

### 1. Data Categories Collected and Processed

| Data Field | Purpose | Necessity Justification | Retention |
|------------|---------|------------------------|-----------|
| DICOM imaging file | Core diagnostic input | Essential — system cannot function without imaging data | 90 days post-report |
| Patient NHS/hospital ID | Patient matching to EHR | Essential — prevents wrong-patient errors in diagnostic workflow | Duration of clinical episode |
| Date of birth | Age-appropriate diagnostic thresholds | Essential — diagnostic baselines differ by age group | Duration of clinical episode |
| Biometric face scan | Patient identity verification at scan | Justified — prevents wrong-patient DICOM association in high-volume radiology departments | Deleted immediately after verification |
| AI-generated report | Clinical audit and accountability | Essential — required for MHRA compliance and radiologist audit trail | 7 years (medical records requirement) |
| Radiologist sign-off record | Accountability and audit | Essential — required to evidence human oversight for regulatory purposes | 7 years |

**Data NOT collected:**
- Patient name (NHS/hospital ID used for matching)
- Address or contact details
- Financial information
- Social history beyond what appears in the EHR extract

---

### 2. Biometric Data Justification

The use of biometric face scans for patient identity verification was subject to a **Data Protection Impact Assessment (DPIA)** completed in March 2026. The DPIA evaluated three alternatives:

| Alternative | Assessment |
|-------------|------------|
| NHS/hospital wristband barcode scan | Rejected — wristbands are frequently removed or misplaced in clinical environments, creating patient safety risk |
| Two-factor staff confirmation | Rejected — adds clinical workflow burden and does not prevent wrong-patient errors in automated overnight batch processing |
| Biometric face scan (selected) | Accepted — provides definitive patient matching with minimal data collected; face scan deleted immediately after verification |

The DPIA concluded that biometric verification is proportionate to the patient safety risk of wrong-patient diagnostic errors in a high-volume radiology environment.

---

### 3. Children's Data Handling

For patients under 18 in paediatric wards:
- The same data minimisation principles apply
- Parental or guardian consent is obtained as part of the hospital admission process under Article 9(2)(h) GDPR (medical diagnosis)
- Paediatric records are stored in a separate logical partition with additional access controls (consultant-only access)
- Face scan biometrics for children under 13 are not collected — ward staff confirmation is used instead

---

### 4. Data Flows Summary

```
Patient → [Face scan verification] → Deleted immediately
Patient → [DICOM image] → MediScan AI inference → AI Report → Radiologist review → Clinical record
Patient → [NHS ID + DOB] → EHR lookup → Contextual data for report → AI Report
```

No patient data is used for model retraining without explicit patient consent and a separate ethics committee approval.

---

### 5. DPIA Reference

A full DPIA for MediScan AI was completed in accordance with UK GDPR Article 35. Reference: **DPIA-MEDISCAN-2026-001**. Available from the Data Protection Officer on request.

**Document Owner:** Data Protection Officer  
**Last Reviewed:** June 2026  
**Classification:** Confidential — Data Governance
