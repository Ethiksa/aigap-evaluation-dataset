# SEC-01: Threat Model

**Identified threats:**
- **Misuse:** A staff member entering identifying student data despite training — mitigated by system prompt design that does not request identifying fields, plus training and periodic review.
- **Unauthorized access:** Someone outside the seven LSO accounts attempting to access the tool — mitigated by SSO restriction to named accounts only (see PRIV-05).
- **Abuse:** Attempting to use the tool for purposes outside its scope (e.g. drafting unrelated correspondence) — mitigated by system prompt scoping and Dr. Marsh's monthly sample review.
- **Adversarial prompt injection:** A staff member attempting to manipulate the system prompt via crafted input — low risk given the closed, trusted user base of seven trained staff; monitored via logging (TRAN-05).

**Owner:** Digital Governance Office, Ashcombe University | June 2026