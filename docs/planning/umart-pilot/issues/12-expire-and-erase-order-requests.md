# 12: Expire and erase Order Requests

Status: ready-for-agent
Blocked by: 11 Discuss, decline, or cancel a request

## What to build

An unanswered Order Request expires at its applicable deadline, leaves normal Orders immediately, and has its request-only records erased seven days later.

## Acceptance criteria

- [ ] Pending and Discussing deadlines use the rules in the pilot spec and are evaluated in Asia/Manila. A message restarts the seven-day inactivity window when no fulfillment start exists.
- [ ] An Expired Order Request disappears from normal buying and selling views at the deadline and cannot be confirmed or messaged as an active request.
- [ ] Seven days after expiry, the request, request-only messages, and associated notices are erased. A separate Listing-level conversation remains.
- [ ] Evidence needed for a seeded open moderation case is held only until case closure; then request evidence is erased, leaving minimal outcome and account-action history.
- [ ] Controlled-time tests cover both deadline types, immediate hiding, erasure, and a case hold and release.

## Comments
