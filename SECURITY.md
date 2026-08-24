# Security and confidentiality

This repository contains anonymized portfolio templates, not production exports.

The following information has intentionally been removed or replaced:

- Credential IDs, names, tokens, secrets, and authentication headers
- Internal API endpoints and cloud-resource URLs
- Database hosts and company-specific schema names
- OneDrive, SharePoint, workbook, worksheet, and table identifiers
- Mailboxes, employee addresses, and company-domain restrictions
- Production room, account, profile, entity, and request identifiers
- Pinned execution data and workflow-instance metadata
- Company-specific Salesforce field names

Before publishing any future n8n export:

1. Obtain the required employer or system-owner approval.
2. Export a duplicate portfolio version, never the active production workflow.
3. Remove credentials and pinned data.
4. replace internal identifiers and endpoints with placeholders.
5. Search the entire export for company names, email addresses, URLs, IDs, tokens, and customer data.
6. Keep the public workflow inactive by default.

If a secret is accidentally committed, deleting it in a later commit is not sufficient. Revoke or rotate it immediately and remove it from the repository history.

