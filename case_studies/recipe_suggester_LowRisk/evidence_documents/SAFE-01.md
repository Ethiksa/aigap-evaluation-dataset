# SAFE-01: Safety Requirements and Harm Scenarios
## RecipeSuggest — Nourish Community Kitchen

**Identified harm scenarios and safeguards:**

| Scenario | Likelihood | Severity | Safeguard |
|----------|------------|----------|-----------|
| Tool suggests recipe containing an allergen present in the kitchen | Low | Medium | System prompt warns about allergens; volunteer trained to always check independently |
| Tool gives impractical suggestion for large-batch cooking | Medium | Low | Volunteer ignores and uses their own knowledge |
| Tool becomes unavailable (API outage) | Low | Minimal | Volunteers cook without the tool — they did so before it existed |
| Volunteer over-relies on tool and stops using own judgment | Low | Low | Limitations clearly stated; tool framed as a thinking aid only |
| Inappropriate or offensive recipe suggestion | Very low | Low | GPT-4o content moderation active; volunteer discards and reports to Sam |

**No safety-critical scenarios identified.** RecipeSuggest has no ability to physically harm anyone, make decisions on anyone's behalf, or affect any person's rights or access to resources.

**Safety requirement:** The tool must always include a reminder that allergens should be checked independently. This is embedded in the system prompt and visible on the tablet screen.

**Owner:** Sam Okafor, Volunteer Coordinator | June 2026
