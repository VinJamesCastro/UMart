# 23: Report Members and activity

Status: ready-for-agent
Blocked by: 05 Review keyword-held Listings, 09 Message from a Listing, 12 Expire and erase Order Requests, 13 Confirm and cancel Transactions

## What to build

A signed-in Member reports a Member, Listing, Order Request, Transaction, message, or conversation with context and private evidence. The founder reviews the allegation and records an outcome.

## Acceptance criteria

- [ ] The report captures target, reason, explanation, related records, and optional screenshot or photo evidence in private storage.
- [ ] The founder/admin sees a protected queue for reports, repeated reports, and suspicious patterns, with status and action history. They can take no action, warn, remove content, restrict, suspend, or record another moderation outcome. Restrictions and suspensions stop the affected account actions.
- [ ] A report or warning sign does not automatically hide a Live Listing. The founder decides whether action is needed.
- [ ] An open case keeps only necessary Expired Order Request evidence; case closure erases it and retains minimal outcome and account-action history.
- [ ] Reporter and moderator access to evidence follows their roles; unrelated Members cannot read it. A moderator can access private Transaction details only while handling a report or support case. Tests cover authorization and the expiry hold and release.

## Comments
