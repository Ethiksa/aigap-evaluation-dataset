# PRIV-01: Data Minimization
**CreditScore AI — FinTrust Bank**

Model inputs: Experian credit file fields (accounts, payment history, utilisation, CCJs, insolvency, enquiries), declared income, employment status, employment length, loan amount and purpose. Explicitly excluded: name, address, date of birth (used for identity verification only), ethnicity, religion, gender. Postcode was evaluated and excluded after bias testing (FAIR-03) showed high proxy-discrimination risk.

**Owner:** Aisha Rahman, DPO