---
name: crm-system
description: Operate PioneerGuard lead capture, channel-separated CRM stages, follow-up, exports, and verified event handoff.
---
# CRM System

## Recorded work
Historical work separated Meta Lead Ads and WhatsApp CTWA sources, tracked CRM stages, exports and event handoff. Notes dated 2026-10-27 recorded limited API-accepted samples; this proves only API acceptance. A later UI grouping repair still needed deployment/read-back verification. Current production state is not asserted.

2026-10-28 source update: CRM detail pages now label the selected view (Lead Ads or WhatsApp CTWA) separately from the original source. CSV export checks the selected channel and stage before download, keeps populated invalid-stage exports available, and stops empty downloads with a user-facing message. The session reports 142 local tests passed. Source changes are not deployed; production behavior remains unverified.

## Workflow
1. Identify source channel and preserve only real source identifiers.
2. Create or match one lead using existing duplicate rules; capture only supplied fields.
3. Advance qualification, opportunity/quote, sample and sale stages only when the real milestone occurs; keep stage history.
4. Export by date, channel and stage; verify filters, row count and fields before sharing.
5. Before event handoff, check stage, source, supported event, matching key, deduplication and channel contract.
6. Save, reopen, inspect live behavior and logs; check API acceptance, platform match, attribution and business outcome separately.

Never equate clicks/raw submissions with qualified demand. Keep customer records and IDs private.
