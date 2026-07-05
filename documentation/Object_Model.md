# Object Model

## Project Name
AI-Powered Customer Support Ticketing System

## Standard Object Used
### Case
The Case object is used to manage customer support tickets.

### Important Fields
| Field Name | Type | Description |
|------------|------|-------------|
| Case Number | Auto Number | Unique identifier for each case |
| Subject | Text | Short description of the issue |
| Description | Long Text | Detailed explanation of the issue |
| Status | Picklist | New, Working, Escalated, Closed |
| Priority | Picklist | High, Medium, Low |
| Contact | Lookup | Customer who raised the case |
| Owner | Lookup | Assigned support agent |

## Relationships
- One Contact can have multiple Cases.
- Each Case is assigned to one Owner.
- Reports are generated from Case records.

## Automation
- Record-Triggered Flow sends an email notification whenever a case is created or updated.
