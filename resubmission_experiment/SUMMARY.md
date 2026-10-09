# Resubmission-Convergence Experiment — GOV-01 (StudySpark AI, Medium Risk tier)

## Protocol
A single control (GOV-01, ownership and accountability) was evaluated, revised to specifically
address every gap identified, and resubmitted — five times — to test whether genuine, targeted
remediation converges the evaluator toward a stable "Ready" determination.

## Result
Across five real evaluation rounds, the control never reached an empty gaps list (the condition
required for a true Ready status). Round 6 (`GOV-01_round6_minimal.md`) was a deliberately
scope-minimized revision, restricted strictly to the content directly requested by the control's
reviewer question, to test whether narrower scope reduces exposure to further gap-finding.
Completing and reporting round 6's result is left to future work.

## Round-by-Round Pattern

| Round | Gap Theme | Character |
|---|---|---|
| 1 | Deputy arrangement, internal communication, review cadence | Genuine structural gap |
| 2 | External communication, ongoing QA, formal role profile | Genuine structural gap |
| 3 | Signed acknowledgement evidence, document verification, complaint escalation path | Onset of evidentiary regress |
| 4 | Full document attachment (vs. extracts), role acceptance confirmation, peer-review schedule | Evidentiary regress |
| 5 | Full document attachment (vs. full in-line text), cross-reference confirmation, **hallucinated truncation claim** | Evidentiary regress + hallucination |

## Key Finding: The Round 5 Hallucination

In round 5, the evaluator asserted that a specific review-cadence reference appeared truncated
mid-sentence. This claim was independently verified against the actual submitted document
(`GOV-01_round5.md`) and found to be **false** — the referenced text was present in full. This is
documented as a distinct failure mode from evidentiary regress: a factually incorrect, checkable
claim about the evaluator's own input, asserted with the same confidence as its other findings.

## Why This Matters

This experiment is the primary empirical basis for this work's central architectural argument:
an LLM evaluator's raw judgment is not a reliable, standalone arbiter of compliance status, and
a deterministic verification layer is necessary — not merely a safeguard against rare error, but
a correction for behavior observed to occur systematically under genuine, repeated, good-faith
remediation.
