# 16: Resolve disputed fulfillment

Status: ready-for-agent
Blocked by: 05 Review keyword-held Listings, 15 Auto-confirm unanswered claims

## What to build

A Buyer disputes a fulfillment claim, and the founder/admin reviews and records whether it stands. The outcome changes Transaction state without creating unearned public credit.

## Acceptance criteria

- [ ] The Buyer can dispute while Awaiting buyer confirmation or within the allowed late-response window after Auto-confirmation.
- [ ] A protected founder/admin view shows the Disputed Transaction and relevant case information; regular Members cannot resolve it.
- [ ] Upholding the claim produces Moderator-verified completion with no public or pilot credit or ratings unless the Buyer later confirms explicitly.
- [ ] Removing a false claim returns the Transaction to Confirmed if both parties continue, or Cancels it otherwise. Any restored capacity follows the usable-capacity rule.
- [ ] Tests cover both outcomes, recorded moderator action, access control, and public count exclusion.

## Comments
