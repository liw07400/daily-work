---
name: whatsapp-capi
description: Maintain WhatsApp CTWA intake-to-CRM and supported Conversions API workflows with separate proof gates.
---
# WhatsApp CTWA + CAPI

## Recorded work
Historical work examined webhook intake, referral identifiers, CRM decisions, event naming, idempotency and event status. Limited API acceptance checks do not prove message delivery, matching, attribution, optimization or sales. Local invalid/junk labels remain local unless verified as supported.

## Workflow
1. Verify current account, webhook, callback, permissions and deployment.
2. Retain an ad/referral ID only when it arrives with the message; never infer or fabricate it.
3. Deduplicate and create/match the CRM record; keep source and message status accurate.
4. Send only a supported event after the real customer milestone; keep local stage names separate from API event names.
5. Apply idempotency and clear pending/accepted/rejected/uncertain status; follow safe retry rules.
6. Verify response, platform receipt/matching, funnel setup, optimization eligibility and campaign results separately.
7. Redact credentials, messages, phone numbers and customer/account IDs.

Asset listing is not webhook intake, message sending or event return. HTTP/API acceptance is not attribution or revenue. Recheck current official API rules before changing payloads.

## Historical event correction — 2026-10-31
- In the recorded SDK review, no supported method was verified for retracting an already received event by `event_id`; obtain confirmation from Meta support before promising deletion or exclusion.
- Separate Meta-side historical correction from local CRM receipt cleanup. Removing local rows, stopping a webhook, changing a shared event name, deleting a dataset or changing WABA bindings does not prove the received Meta event was removed; keep unrelated WhatsApp flows intact unless separately authorized and verified.
