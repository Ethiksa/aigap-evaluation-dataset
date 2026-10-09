# TRAN-04: Model Card — RecipeSuggest
## Nourish Community Kitchen | June 2026

**System name:** RecipeSuggest
**Model used:** OpenAI GPT-4o (via API)
**Deployed by:** Nourish Community Kitchen volunteers
**Intended users:** Kitchen volunteers only (2 people)

### Intended Use
Suggest up to three recipes based on a typed ingredient list during meal preparation sessions at Nourish Community Kitchen.

### Out-of-Scope Use
Food safety decisions, allergen management, meal planning for individuals with medical dietary needs, any use involving personal data, any use outside the kitchen volunteer team.

### Data
No training data from Nourish Community Kitchen. No fine-tuning performed. The system uses a system prompt with kitchen-specific instructions. Ingredient lists are sent per-query and not retained.

### Known Limitations
- Does not know about allergens unless volunteers ask explicitly
- Does not know available kitchen equipment
- May suggest impractical recipes for large-batch community cooking
- English language only
- No memory between queries

### Risk Level
Minimal. Informational only. No decision-making capability.

### Version
1.0 — June 2026 | **Owner:** Sam Okafor, Volunteer Coordinator
