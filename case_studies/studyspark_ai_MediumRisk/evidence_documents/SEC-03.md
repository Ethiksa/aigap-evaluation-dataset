# SEC-03: Secure Development Practices

**Dependencies:** The tool uses the official Azure OpenAI SDK, kept up to date via the Digital Governance Office's standard patching schedule (monthly).

**Secrets management:** The Azure OpenAI API key is stored in Azure Key Vault, never in application code or version control, and rotated every 90 days (see PRIV-05).

**Code review:** The tool's codebase, maintained by the Digital Governance Office development team, follows the university's standard code review process requiring at least one peer review before any change is deployed to the production pilot.

**Release hygiene:** Changes are deployed first to a staging environment used by Dr. Marsh for verification before being released to the live staff-facing tool.

**Owner:** Digital Governance Office, Ashcombe University | June 2026