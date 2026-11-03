---
name: email-automation
description: Verify PioneerGuard business email workflows with evidence, prepare safe drafts, and keep sending and deliverability claims bounded.
---
# Email Automation

## Recorded status

2026-10-28: SMTP transport to `smtp.zoho.com` on ports 465 and 587 completed SMTP greeting, TLS 1.3 negotiation and certificate validation. The current account SMTP AUTH, actual send, inbox receipt, IMAP and reply handling remain unverified. Original sending scripts and raw logs were not found. A prior text snapshot records 12 `Sent` and 0 `Failed` on 2026-08-04, but cannot be revalidated from original logs; treat as historical and pending verification. No email was sent in the 2026-10-28 session.

The same session drafted a Zoho workflow for inbox classification, reviewed reply drafts and manual follow-up. Google Trends timed out during country comparison, so no country ranking or search-volume claim is recorded.

## Workflow

1. Confirm the sender, mailbox provider, domain and user-authorized test scope; never request or store passwords, one-time codes, app passwords or cookies in shared notes.
2. Locate the existing sending script and source logs before changing providers or inferring that a prior workflow failed. If unavailable, state that gap.
3. Test DNS/connection, SMTP greeting, TLS certificate, account authentication, message submission, recipient receipt and reply handling as separate gates. A TCP/TLS pass does not prove credentials, sending or deliverability.
4. Verify current provider plan and acceptable-use policy from dated official sources. Do not infer marketing or unattended sending permission from SMTP availability.
5. Prefer inbox rules, reviewed drafts and a human follow-up queue for B2B inquiries. Use D0/D3/D7/D14 as a manual cadence only when appropriate; confirm each message against the real lead and stop when the recipient opts out.
6. Keep mailbox identity, recipient data, message logs, secrets and local paths out of public knowledge. Record only sanitized evidence filenames and status.
7. Report actual message sent, delivered, received and replied as separate outcomes; never claim a complete email loop from a connection test.
