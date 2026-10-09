# FAIR-01: Protected Characteristics and Fairness Risk
## MediScan AI — Model Fairness Assessment (MFAR-MEDISCAN-2026-001)

**Patient groups at elevated diagnostic accuracy risk:**

| Group | Risk | Mitigation |
|-------|------|-----------|
| South Asian patients (Sri Lanka network) | Base model trained on Western datasets; TB presentation may differ | Supplementary fine-tuning with Sri Lanka hospital data 2023–2025 |
| Paediatric patients under 12 | Lung anatomy differs from adult training data | AI output flagged as indicative only; mandatory senior radiologist review |
| Patients with comorbidities | Complex imaging patterns underrepresented in training | Explicit radiologist guidance documentation for multi-condition cases |

**Protected characteristics confirmed not used as model inputs:** Age, sex, ethnicity, religion.

**Ongoing monitoring:** Diagnostic accuracy by demographic group reviewed quarterly by Clinical Governance Lead. Any disparity exceeding 5% triggers model review.

**Document Owner:** Head of AI Engineering | June 2026
