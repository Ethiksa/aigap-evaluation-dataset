# SEC-06: Pre-Trained Model Supply Chain Security
## MediScan AI — LLaMA Vision Supply Chain Assessment (SEC-ASSESS-2026-001)

**Base model:** Meta LLaMA Vision (fine-tuned for pulmonary imaging).

**Provenance:** Obtained from Meta official model repository with SHA-256 checksum verification. Fine-tuning conducted on controlled infrastructure with access limited to the AI Engineering team.

**Known bias assessment:** Meta LLaMA Vision model card reviewed. Gap identified: limited South Asian imaging representation. Mitigation: supplementary fine-tuning with Sri Lanka hospital dataset 2023–2025.

**Adversarial vulnerability assessment:** Evaluated against known adversarial medical imaging attack patterns. No critical vulnerabilities identified for chest imaging use case.

**Security patch process:**
- Meta security advisories monitored weekly.
- Critical patches evaluated within 7 days.
- Model redeployment after any patch requires Clinical AI Review Board approval and clinical re-validation.

**Version management:** Deployed model version pinned in configuration. Changes require formal change request.

**Document Owner:** Head of AI Engineering | June 2026
