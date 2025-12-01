# Email CLAPIT™
## Automated Pharmaceutical Communication Assistant
Email CLAPIT™ is a workflow automation system designed to help pharmaceutical commercial, medical affairs, and partnership teams manage email communication with precision, consistency, and zero missed follow-ups.

Built on n8n, Gmail API, and PostgreSQL, it tracks email threads, detects intent, schedules follow-ups, and sends professional replies using deterministic templates (with optional AI drafting).

## Why I Built This
Pharmaceutical communication involves time-sensitive clarifications, partner follow-ups, internal approvals, and scheduled responses.
As inboxes grow, critical messages get buried — leading to delays that impact contracts, compliance, and decision-making.

Email CLAPIT™ solves this by:

- Watching every incoming email

- Detecting intent (keyword-based)

- Applying a strict follow-up cadence

- Auto-responding with professional templates

- Logging every action to maintain audit-ready traceability

- It removes the manual workload while preserving accuracy and compliance.

  ## Core Features
  ✓ Keyword-Based Intent Detection

Automatically classifies emails into categories like:

- Follow-Ups

- Clarifications

- Scheduling

- Calls / Meetings

- Status updates

- Partner questions

✓ Smart Follow-Up Cadence

- Configurable timing rules:

- 1st follow-up: 25 minutes

- 2nd: 24 hours

- 3rd: 48 hours

- Stop at 3 for compliance safety

✓ Thread-Level Memory (PostgreSQL)

Stores:

- thread_id

- follow_up_count

- last_contacted

- automation_type

- timestamps

✓ Professional Pharma-Tone Templates

Each automation type is paired with a clean, compliant email response.

✓ Optional AI Drafting

Uses OpenAI GPT-4o-mini through a single unified node (optional).

✓ Compliance-Friendly Logging

Tracks every image sent for audit and reporting.

## Tech Stack
<img width="701" height="277" alt="clapit-doc-image" src="https://github.com/user-attachments/assets/9bef7adf-d1da-4624-b2bd-8e13762fd3cc" />

## How It Works
- Trigger: Gmail "New Email" trigger

- Fetch Message (FULL) for reliable parsing

- Extract metadata → subject, body, sender, threadId

- Keyword Detection for automation routing

- Thread Lookup (email_tracking table)

- Decision Logic → Should we follow up? When?

- Template or AI Draft

- Send Email (Gmail SMTP/API)

- Increment follow_up_count and log activity

## Internal Pilot Results
- 85% reduction in follow-up latency

- Operations lead went from 7 hrs/week → <1 hr/week

- Zero missed clarifications

- More predictable partner communication

 ## 🏆 Value Proposition
<img width="551" height="253" alt="image" src="https://github.com/user-attachments/assets/d904ad5a-619f-438b-bcc8-bd42841a8762" />

## Use Cases

- Pharmaceutical commercial teams

- Partnership and vendor management

- Medical affairs follow-ups

- Regulatory communication tracking

- Internal reminders & status updates

  ## License
  MIT License — free to use, extend, and customize.

  ## Contact
  If you'd love to integrate Email CLAPIT™ into your workflow or need customization:

[Email Me](mailto:ismailabdulrahman555@gmail.com)

[🔗 LinkedIn: Message me anytime](https://www.linkedin.com/in/ismail-abdulrahman)

## Watch Demo
https://drive.google.com/file/d/1fe9l5fH7WmYfWKVJDn4BTvJGq4MucV1h/view?usp=sharing
