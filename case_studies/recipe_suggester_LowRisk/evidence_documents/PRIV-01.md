# PRIV-01: Data Minimisation
## RecipeSuggest — Nourish Community Kitchen

**Data sent to OpenAI API:** Only the ingredient list typed by the volunteer in that session. For example: "carrots, onions, lentils, cumin, tinned tomatoes."

**No personal data is collected or processed.** The ingredient list contains no names, no identifying information, no health data, and no information about any individual person.

**Data excluded by design:**
- Names or details of kitchen visitors or meal recipients — never entered
- Any dietary or health information about individuals — the volunteer handles this separately using their own knowledge, not the tool
- Location data, contact details, or any other personal identifiers

**Session behaviour:** Each query is independent. The tool has no memory of previous queries. When the tablet screen is cleared, nothing is retained.

**OpenAI configuration:** The zero data retention API option is enabled on the Nourish Community Kitchen OpenAI account, meaning query text is not stored by OpenAI after the API response is returned.

**Owner:** Sam Okafor, Volunteer Coordinator | June 2026
