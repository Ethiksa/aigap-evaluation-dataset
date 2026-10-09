# DOC-01: System Description Pack
## RecipeSuggest — Nourish Community Kitchen | June 2026

### Purpose
RecipeSuggest is an AI recipe suggestion tool that helps kitchen volunteers at Nourish Community Kitchen decide what to cook based on the ingredients available that day.

### Users
Two kitchen volunteers at Nourish Community Kitchen. No other users.

### Scope
Ingredient-to-recipe suggestions during meal preparation sessions only.

### Out of Scope
Food safety decisions, allergen management for individuals, personal data processing, use by anyone outside the kitchen volunteer team, any deployment beyond the single kitchen tablet.

### System Architecture
- Interface: Simple text input web app on an Android tablet
- Model: OpenAI GPT-4o via API
- System prompt: Kitchen-specific instructions including allergen warning and three-recipe limit
- Authentication: None required — tablet is physically located in the kitchen
- Data retention: None — stateless; OpenAI zero retention API option enabled

### Assumptions
- Volunteers have practical cooking experience and will not blindly follow suggestions
- Volunteers will check allergens independently regardless of what the tool suggests
- The tablet remains in the kitchen and is not used for any other purpose

### Known Limitations
- English language only
- No knowledge of individual dietary needs
- No knowledge of available equipment
- No memory between sessions
- May suggest impractical large-batch recipes

### Version
1.0 — June 2026 | **Owner:** Sam Okafor, Volunteer Coordinator
