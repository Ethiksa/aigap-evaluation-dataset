# SAFE-04: Fallback Behavior
**CreditScore AI — FinTrust Bank**

If the model produces a low-confidence score (bottom decile of prediction confidence) or the Experian API fails, the application routes to full manual underwriting rather than a forced automated score, consistent with HUMO-04.

**Owner:** Dr. Wei Tan, Head of Model Risk