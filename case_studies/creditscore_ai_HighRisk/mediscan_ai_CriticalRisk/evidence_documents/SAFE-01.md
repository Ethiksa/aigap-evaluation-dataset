# SAFE-01: Harm Scenario Identification
## MediScan AI — Harm Scenario Register (HSR-MEDISCAN-2026-001)

| # | Scenario | Severity | Mitigation |
|---|----------|----------|-----------|
| 1 | False negative cancer detection — system fails to flag lung cancer nodule | Critical | High-sensitivity calibration; mandatory radiologist review of all outputs |
| 2 | False positive — benign finding flagged as high-risk, leading to unnecessary biopsy | High | Confidence score thresholds documented in radiologist guidance |
| 3 | System unavailability during time-critical emergency presentation | High | System is advisory only; radiology workflow proceeds without AI if unavailable |
| 4 | Wrong-patient diagnostic error — AI report attached to incorrect record | Critical | Biometric face scan verification before image upload; PACS dual-check |
| 5 | Model performance degradation over time causing systematic misdiagnosis | High | Monthly performance monitoring with automated drift detection alerts |

**Review cycle:** Harm scenario register reviewed at every Clinical AI Review Board meeting (quarterly).

**Document Owner:** Chief Medical Officer | June 2026
