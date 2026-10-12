# AIGAP Evaluation Dataset

Real evaluation outputs from AIGAP's AI Design Reviewer and Risk Classifier — a hybrid LLM-deterministic
pipeline for automated AI governance evidence evaluation — across four real project case studies spanning
the full risk spectrum, plus a controlled resubmission-convergence experiment.

## Risk Tiers

AIGAP evaluates projects against a cohort-based control registry with four risk tiers:

| Tier (current naming) | Controls Active |
|---|---|
| Low Risk | 19 |
| Medium Risk | 42 |
| High Risk | 76 |
| Critical Risk | 84 |

## What's Inside

| Folder | Case Study | Tier | Controls Evaluated | Real Pipeline Run? |
|---|---|---|---|---|
| `case_studies/recipe_suggester_LowRisk/` | RecipeSuggest — ingredient-to-recipe tool | Low Risk | 19 of 19 | Yes |
| `case_studies/studyspark_ai_MediumRisk/` | StudySpark AI — university staff drafting assistant | Medium Risk | 42 of 42 | Yes |
| `case_studies/creditscore_ai_HighRisk/` | CreditScore AI — bank credit risk scoring | High Risk | 76 of 76 | Yes |
| `case_studies/mediscan_ai_CriticalRisk/` | MediScan AI — clinical imaging diagnostic assistant | Critical Risk | 13 (representative subset of 84) | Yes |
| `resubmission_experiment/` | Five-round resubmission trace on a single control (GOV-01) | Medium Risk | 1 control, 5 rounds | Manual, iterative |

Each case study folder contains:
- `input_profile.json` — the project's intake profile and active control set
- `crp.json` — full Certification Readiness Plan output (per-control status, gaps, strengths, reasoning)
- `risk_classifier.json` — risk classification output (adjusted score, triggered regulations, recommendations)
- `pipeline_summary.json` — run metadata (cost, tokens, status distribution)
- `evidence_documents/` — the actual governance evidence submitted per control

**Note:** `creditscore_ai_HighRisk` currently contains the full 76-control evidence set and input
profile but not yet a completed pipeline run output — this is noted honestly rather than fabricated.
`mediscan_ai_CriticalRisk` does not yet include a `risk_classifier.json` for the same reason.

## Key Findings

- Across all controls evaluated in completed runs, **not a single control ever received an empty
  gaps list** — the condition required for a true "Ready" status was never reached.
- The deterministic rules engine overrode the LLM's own "Ready" judgment in **83.3%** of evaluated
  controls (Low Risk), **59.5%** (Medium Risk), and **30.8%** (Critical Risk subset) — meaning a
  substantial fraction of controls would have been incorrectly certified Ready without this layer.
- The resubmission experiment documents an **evidentiary regress** pattern — repeated, genuine
  remediation triggers progressively deeper requests for proof — and one confirmed instance of the
  evaluator **hallucinating** a false, checkable defect in its own input (see
  `resubmission_experiment/SUMMARY.md`).

## How to Read a CRP File

Each control entry in `crp.json` includes: `reviewer_question`, `rag_context` (retrieved regulatory
text), `llm_evaluation` (`adequacy_score`, `gaps`, `strengths`, `reasoning`), `status` (the final,
deterministically-assigned outcome), and `status_rule_applied` (which of the four D7 rules produced
that outcome).

## Citation

If you use this dataset, please cite it using the metadata in `CITATION.cff`, or see the associated
paper: *"The Evidentiary Regress Problem in LLM-Assisted Compliance Evaluation for AI Governance."*

## License

Released under CC BY 4.0 — see `LICENSE`.

## Contact

Questions or issues — open a GitHub issue on this repository.
