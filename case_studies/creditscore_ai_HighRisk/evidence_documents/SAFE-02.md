# SAFE-02: Testing Against Edge Cases
**CreditScore AI — FinTrust Bank**

Stress tests include: applicants with zero credit history, applicants with recent bankruptcy discharge, applicants with conflicting Experian data fields, and joint applications with mismatched credit profiles. Each edge case is verified to produce a sensible score band or a graceful fallback to manual underwriting rather than an erroneous extreme score.

**Owner:** Dr. Wei Tan, Head of Model Risk