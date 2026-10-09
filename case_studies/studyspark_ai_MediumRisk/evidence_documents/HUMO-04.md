# HUMO-04: Safe Fallback Behaviour

**Fallback scenario:** If the OpenAI API is unavailable or returns an error, StudySpark AI displays: "Draft generation is currently unavailable. Please write your message directly." No partial or malformed draft is ever shown.

**Uncertainty handling:** The system prompt instructs the model to note when it lacks enough context to draft a confident suggestion (for example, if the difficulty description is very brief), in which case it returns a short prompt asking the staff member to add more detail rather than guessing.

**Owner:** Dr. Fiona Marsh, Head of Learning Support | June 2026