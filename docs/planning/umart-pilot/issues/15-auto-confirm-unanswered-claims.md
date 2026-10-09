# 15: Auto-confirm unanswered claims

Status: ready-for-agent
Blocked by: 14 Claim and confirm fulfillment

## What to build

An unanswered fulfillment claim closes as Auto-confirmed completion after 72 hours, while the Buyer retains a seven-day window to respond inside the Transaction.

## Acceptance criteria

- [ ] The system closes an unanswered claim at 72 hours without counting it publicly or unlocking ratings.
- [ ] For seven days after Auto-confirmed completion, the Buyer can still explicitly confirm or dispute in the Transaction; a Buyer confirmation earns credit only then.
- [ ] After that late-response window, the Transaction directs objections to reporting rather than reopening an in-Transaction response.
- [ ] Both participants can distinguish Auto-confirmed from Buyer-confirmed completion in private history.
- [ ] Controlled-time tests cover the 72-hour boundary and the later seven-day boundary.

## Comments
