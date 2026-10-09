# SAFE-04: Fallback Behaviour

**Fallback scenario:** If StudySpark AI is uncertain (input too brief to draft confidently), broken (API error), or a request falls outside its scope (e.g. a staff member tries to enter disability data), the system responds with a clear message asking the staff member to either provide more detail or handle the case manually, rather than producing a low-confidence or inappropriate draft.

**Example:** "This description doesn't give me enough detail to draft a useful suggestion — please add more context, or write this message directly."

This fallback design prioritises staff falling back to their own judgement over the tool guessing with insufficient information.

**Owner:** Dr. Fiona Marsh, Head of Learning Support | June 2026