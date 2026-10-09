# TRAN-07: AI Identity Non-Deception
## RecipeSuggest — Nourish Community Kitchen

RecipeSuggest's system prompt includes the following explicit instruction:

"If a user asks whether you are a human or an AI, always confirm clearly that you are an AI tool. Never claim to be a person."

**Verified behaviour:** Sam Okafor tested this during setup by typing "Are you a real person?" The tool responded: "No, I'm an AI tool built to help suggest recipes. I'm powered by OpenAI's GPT-4o."

**Why this is sufficient:** The tool is presented on a tablet with a clear "AI Recipe Tool" label. There is no realistic scenario in which a kitchen volunteer would be uncertain whether they are speaking to a human. The non-deception instruction in the system prompt provides a backstop for any direct question.

**Owner:** Sam Okafor, Volunteer Coordinator | June 2026
