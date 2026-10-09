# 13: Confirm and cancel Transactions

Status: ready-for-agent
Blocked by: 12 Expire and erase Order Requests

## What to build

A Seller confirms final Marketplace terms, turning a live Order Request into a Transaction and committing stock. Either participant can later cancel the Confirmed Transaction with a reason and notice.

## Acceptance criteria

- [ ] Confirmation freezes final quantity, price, schedule, and handoff, and notifies the Buyer. It requires no separate Buyer acceptance.
- [ ] The Seller can choose which pending request to confirm, regardless of submission order. Confirmation checks and commits available stock in one operation, so two competing confirmations cannot claim the same last unit.
- [ ] A sold-out one-off Listing stops taking new requests. Other pending requests remain visible to their Buyers until manually declined or expired.
- [ ] Confirmed terms cannot be edited in place; a correction uses cancellation and a new Order Request.
- [ ] On cancellation, the Seller chooses a usable amount to restore, capped by the committed amount; cancellation records a reason and notifies the other party. Tests cover competing confirmations, fixed terms, and stock restoration.

## Comments
