# SEC-01: Access Controls
## MediScan AI — Access Control Framework

**Authentication:** NHS-federated SSO using smart card. No username/password login permitted.

**Role-based access control:**

| Role | Access Level |
|------|-------------|
| Consultant Radiologist | Full read and write on assigned cases |
| Radiographer | Image upload only |
| Clinical Governance Lead | Audit log read-only |
| System Administrator | Configuration only, no patient data access |

**Paediatric data restriction:** Under-18 patient records held in a separate logical partition. Access requires Radiologist role plus explicit paediatric authorisation from Clinical Governance Lead.

**Audit logging:** All AI report views, sign-offs, and access events logged to tamper-evident audit log. Retained 7 years per NHS records management standards. Structured for MHRA post-market surveillance under UK MDR 2002 Article 83.

**Document Owner:** Head of AI Engineering | June 2026
