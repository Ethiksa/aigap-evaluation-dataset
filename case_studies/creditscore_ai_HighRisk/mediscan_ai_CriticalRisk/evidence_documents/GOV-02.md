# AIGAP Evidence Artifact: GOV-02
## Documented Purpose, Scope, and Operational Limits
### MediScan AI — Clinical Diagnostic Imaging Assistant

---

### 1. Intended Purpose

MediScan AI is a clinical decision support tool designed to assist radiologists in detecting early-stage pulmonary conditions from chest X-rays and CT scans. The system is not a standalone diagnostic device — it produces advisory clinical decision support reports which must be reviewed and confirmed by a qualified radiologist before any clinical action is taken.

**Validated conditions:**
- Early-stage lung cancer (Stage I and II nodule detection)
- Community-acquired pneumonia
- Pulmonary tuberculosis

**Validated imaging modalities:**
- Posterior-anterior chest X-ray (DICOM format)
- CT thorax with and without contrast

---

### 2. Intended Users

| User Type | Role | Access Level |
|-----------|------|--------------|
| Consultant Radiologist | Review and sign off AI reports | Full |
| Radiographer | Image acquisition and upload | Upload only |
| Clinical Governance Lead | Audit and performance review | Read-only audit |
| System Administrator | Configuration and access management | Admin |

MediScan AI is not intended for use by patients, general practitioners without radiology training, or any clinical staff outside of the radiology and respiratory medicine departments.

---

### 3. Explicit Out-of-Scope Uses

The following uses are explicitly prohibited and technically blocked where feasible:

- **Autonomous diagnosis:** MediScan AI must never be used to make a final diagnosis without radiologist review. Its outputs are advisory only.
- **Emergency triage without oversight:** The system must not be used as the sole assessment tool in time-critical emergency presentations where radiologist review is unavailable.
- **Paediatric bone age or non-pulmonary imaging:** The system is validated for pulmonary imaging only. Use on non-chest imaging modalities is prohibited.
- **Legal or insurance documentation:** MediScan AI outputs must not be cited in legal proceedings or insurance assessments as standalone evidence.
- **Deployment outside validated environments:** The system must not be used in clinical environments that have not completed the validated deployment configuration checklist.

---

### 4. Limits of Assessment Authority

MediScan AI produces a **Clinical Decision Support Report** containing:
- A confidence-scored finding for each validated condition
- A recommended action flag (Urgent Review / Routine Review / No Finding)
- A structured list of imaging features that contributed to the finding

**The system explicitly does not:**
- Issue prescriptions or treatment recommendations
- Override radiologist clinical judgment
- Produce outputs that constitute a certified medical diagnosis
- Store any clinical decision without radiologist attribution

---

### 5. Regulatory Classification

MediScan AI is classified as a **Class IIa medical device** under UK MDR 2002 and has been registered with the MHRA prior to deployment. The CE marking transition plan under UKCA is documented separately in the regulatory compliance register.

**Document Owner:** Chief Medical Officer  
**Last Reviewed:** June 2026  
**Classification:** Confidential — Clinical Governance
