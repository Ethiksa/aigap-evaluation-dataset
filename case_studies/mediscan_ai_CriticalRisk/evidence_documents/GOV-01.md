# AIGAP Evidence Artifact: GOV-01
## Ownership and Accountability Statement
### MediScan AI — Clinical Diagnostic Imaging Assistant

---

### 1. Named Accountable Owner

The named accountable owner for MediScan AI is the **Chief Medical Officer (CMO)**, currently Dr. Ananya Perera, who holds personal accountability for all clinical governance decisions relating to the system.

**Accountability scope includes:**
- Clinical validity of AI-assisted diagnostic outputs
- Patient safety decisions arising from system failures or performance degradation
- Regulatory compliance with MHRA Medical Device Regulations 2002
- Cross-border governance alignment between UK and Sri Lanka networks

A secondary technical owner, the **Head of AI Engineering**, holds accountability for system infrastructure, model version management, and security controls.

---

### 2. Accountability Governance Structure

| Role | Accountability Area | Escalation Path |
|------|---------------------|-----------------|
| Chief Medical Officer | Clinical safety, patient harm, MHRA reporting | Hospital Board |
| Head of AI Engineering | Model performance, infrastructure, security | CTO |
| Clinical Governance Lead (UK) | Radiologist oversight, audit compliance | CMO |
| Clinical Governance Lead (LK) | Sri Lanka network compliance, LK PDPA | CMO |
| Data Protection Officer | GDPR/UK GDPR compliance, cross-border transfers | CMO + Legal |

---

### 3. Accountability Across Design, Deployment, and Post-Deployment

**Design Phase:** The CMO approved the clinical intended use statement and harm scenario register prior to pilot deployment. All design decisions that affect diagnostic outputs require CMO sign-off via the Clinical AI Review Board.

**Deployment Phase:** The Head of AI Engineering is accountable for deployment configuration, including model version pinning, API access controls, and PACS/EHR integration security. No production deployment proceeds without a signed Clinical AI Deployment Authorisation from the CMO.

**Post-Deployment:** Monthly clinical performance reviews are chaired by the CMO. The Clinical Governance Leads in each network submit quarterly reports covering: diagnostic accuracy metrics, false negative and false positive rates, radiologist satisfaction with AI outputs, and any adverse event reports.

---

### 4. Escalation and Accountability Chain

If a patient harm event is associated with a MediScan AI output:
1. The attending radiologist reports to the Clinical Governance Lead within 24 hours
2. The Clinical Governance Lead notifies the CMO within 48 hours
3. The CMO activates the incident response protocol and notifies MHRA within 15 days (as required under UK MDR 2002)
4. The Head of AI Engineering suspends the affected model version pending investigation

---

### 5. Review and Renewal

This accountability statement is reviewed annually by the Clinical AI Review Board and updated within 30 days of any change to the named accountable owner or governance structure.

**Document Owner:** Chief Medical Officer  
**Last Reviewed:** June 2026  
**Next Review:** June 2027  
**Classification:** Confidential — Clinical Governance
