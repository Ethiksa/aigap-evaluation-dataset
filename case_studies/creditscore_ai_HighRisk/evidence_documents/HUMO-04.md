# HUMO-04: Safe Fallback Behaviors Implemented
**CreditScore AI — FinTrust Bank**

If the Experian API is unavailable or the model fails to return a score, the application is routed to full manual underwriting rather than blocked or defaulted to any score value. No application is ever auto-declined due to a system failure.

**Owner:** Dr. Wei Tan, Head of Model Risk