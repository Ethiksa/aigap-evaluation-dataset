# PRIV-04: Data Retention and Deletion
## RecipeSuggest — Nourish Community Kitchen

**No data is retained by the system.** RecipeSuggest is stateless — each ingredient query is sent to the OpenAI API and the recipe suggestion is displayed on screen. Nothing is saved to the tablet, to any database, or to any file.

**OpenAI retention:** The zero data retention API option is enabled. OpenAI does not store the ingredient query text after returning the response.

**Deletion:** Because no data is stored, no deletion process is required or applicable.

**Logs:** No usage logs are created. The tablet does not record which queries were made or when.

**Review:** Sam Okafor checks the OpenAI account settings annually to confirm zero retention remains active.

**Owner:** Sam Okafor, Volunteer Coordinator | June 2026
