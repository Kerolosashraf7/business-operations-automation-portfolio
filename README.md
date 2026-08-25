# Business Operations Automation Portfolio

This repository presents four anonymized workflow-automation projects built with n8n. They demonstrate how I translate manual operational processes into controlled, observable, and recoverable integrations across email, spreadsheets, databases, APIs, CRM systems, and cloud messaging.

> The workflows are portfolio templates. Production credentials, URLs, resource identifiers, company data, and proprietary system names have been removed or replaced with placeholders.

## Projects

| Project | Business outcome | Main integrations |
| --- | --- | --- |
| [Bulk Feedback Publication Automation](projects/bulk-feedback-publication/) | Converts an authorized email and CSV request into a validated bulk database update with a single outcome reply. | Outlook, CSV, Microsoft SQL Server |
| [Reviews and Ratings Migration Automation](projects/reviews-ratings-migration/) | Safely migrates profile reviews and ratings while preventing duplicates and supporting checkpoint-based recovery. | Excel 365, SQL Server, REST API, AWS SQS |
| [Profile Ranking Operations Automation](projects/profile-ranking-operations/) | Processes bulk ranking adjustments from email, synchronizes database and API state, optionally updates CRM, and returns one consolidated report. | Outlook, CSV, MySQL, REST API, Salesforce |
| [Sandbox Account Provisioning Automation](projects/sandbox-account-provisioning/) | Converts a sandbox email and CSV request into validated API-based account provisioning with one row-level outcome report. | Outlook, CSV, REST API |

## Skills demonstrated

- Business-process analysis and workflow architecture
- Event-driven and scheduled automation
- OAuth-based Microsoft 365 integrations
- CSV and Excel-based intake design
- SQL Server and MySQL data operations
- REST API integration and response validation
- Salesforce record lookup and updates
- AWS SQS messaging
- Batch and per-item processing
- Idempotency and duplicate prevention
- Transactional data updates
- Checkpointing and resumable workflows
- Validation, branching, retries, and controlled failure paths
- Consolidated business notifications and audit-friendly statuses
- Production troubleshooting and operational hardening

## Design principles

The projects use a consistent set of engineering principles:

1. Validate requests before changing downstream systems.
2. Isolate each request so one failure does not corrupt another.
3. Verify database state after each critical update.
4. Avoid duplicate or unsafe writes.
5. Preserve a clear status for success, blocked, and review-required outcomes.
6. Retry temporary service failures without hiding permanent errors.
7. Return concise, useful results to the requesting team.

## Using the workflow templates

The included JSON files are inactive and contain placeholders. After importing one into n8n, select your own credentials and replace all values beginning with `REPLACE_WITH_`. The schemas and example endpoints are intentionally generic and must be mapped to your environment.

See [SECURITY.md](SECURITY.md) before using or sharing any workflow export.

## Repository topics

Suggested GitHub topics:

`n8n` `workflow-automation` `business-process-automation` `api-integration` `account-provisioning` `salesforce` `sql-server` `mysql` `microsoft-365` `aws-sqs` `csv-processing`

