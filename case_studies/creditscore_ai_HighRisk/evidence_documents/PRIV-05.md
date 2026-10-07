# PRIV-05: Access Control and Least Privilege
**CreditScore AI — FinTrust Bank**

Access via Azure AD SSO with MFA; loan officers view only applications assigned to them, enforced at the API layer. Score queries are logged with user ID, timestamp, and application ID, retained 7 years for FCA compliance. Experian API credentials are stored in Azure Key Vault, rotated every 90 days.

**Owner:** Digital Governance Office