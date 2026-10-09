# 14: Claim and confirm fulfillment

Status: ready-for-agent
Blocked by: 13 Confirm and cancel Transactions

## What to build

The Seller can update a physical order as ready for pickup, claim fulfillment of a Confirmed Transaction, and receive the Buyer's explicit confirmation.

## Acceptance criteria

- [ ] Ready for pickup is a fulfillment update, not a completion claim or public completion credit.
- [ ] A fulfillment claim moves the Transaction to Awaiting buyer confirmation, alerts the Buyer, and shows the 72-hour response deadline.
- [ ] Only the Buyer can explicitly confirm the claim. That creates Buyer-confirmed completion and public completion credit.
- [ ] Both participants see current state and frozen terms in their private histories. A third Member cannot read them.
- [ ] Tests distinguish ready, claimed, and Buyer-confirmed states and verify no stock restoration on completion.

## Comments
