# 17: Publish transaction-linked reputation

Status: ready-for-agent
Blocked by: 14 Claim and confirm fulfillment

## What to build

After Buyer-confirmed completion, the Buyer and Seller can each optionally leave one rating and review, shown under separate public buyer and seller/provider reputation summaries.

## Acceptance criteria

- [ ] Each participant can submit at most one rating and review per Buyer-confirmed Transaction, in the correct author role.
- [ ] A fulfillment claim or any completion without explicit Buyer confirmation cannot unlock a rating or increase a public completed-Transaction count.
- [ ] Profiles show separate buyer and seller/provider averages, rating counts, reviews, and Buyer-confirmed completion counts.
- [ ] Public reviews do not expose room numbers, contact information, private terms, or conversation content; a moderator can remove abusive or fabricated reviews.
- [ ] Tests cover both rating directions, duplicate prevention, privacy, and ineligible Transaction states.

## Comments
