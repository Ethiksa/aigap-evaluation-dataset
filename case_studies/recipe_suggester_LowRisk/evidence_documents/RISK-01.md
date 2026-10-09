# RISK-01: System Context
## RecipeSuggest — Nourish Community Kitchen

**Domain:** Community food preparation — general utility tool.

**Stakeholders:**
- Kitchen volunteers (2 people) — direct users
- Kitchen visitors receiving meals — indirectly affected by what gets cooked, but not by the AI tool itself

**Scale:** 2 users. Estimated 3–5 queries per cooking session, 2–3 sessions per week.

**Decision impact:** None. The tool suggests recipes. The volunteer decides what to cook based on their own judgment, available equipment, and knowledge of any dietary needs of guests. The AI output is one informal input among many.

**Operating environment:** Single Android tablet in the kitchen. Wi-Fi for OpenAI API only. No other network connections. No shared accounts or login — the app opens directly on the tablet.

**Dependencies:** OpenAI GPT-4o API. No other external services.

**Owner:** Sam Okafor, Volunteer Coordinator | June 2026
