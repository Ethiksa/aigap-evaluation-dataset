# DOC-01: System Description Pack

### Purpose
StudySpark AI drafts suggested study guidance messages for LSO staff to review and send to students.

### Users
7 LSO staff members at Ashcombe University.

### Scope
Drafting assistance for student guidance messages during the Learning Support process.

### Out of Scope
Direct student communication, decision-making, use outside the LSO, entry of disability or health data.

### System Architecture
- Interface: Internal web tool, SSO-gated
- Model: Azure OpenAI GPT-4o (EU region)
- Data retention: None — stateless, hashed logging only for usage volume
- Authentication: University SSO, restricted to 7 named accounts

### Assumptions
Staff will always review and personalise drafts; the tool will never gain direct student messaging capability without a fresh risk assessment.

### Limitations
No memory between sessions; no access to student information system; English only.

### Version
1.0 — June 2026 | **Owner:** Dr. Fiona Marsh, Head of Learning Support