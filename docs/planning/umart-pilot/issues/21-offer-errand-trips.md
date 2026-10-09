# 21: Offer Errand Trips

Status: ready-for-agent
Blocked by: 13 Confirm and cancel Transactions

## What to build

A Provider publishes a reusable Errands / Pasabuy Listing with dated Errand Trips. A Buyer can request a trip and receive a confirmed Transaction against its remaining capacity.

## Acceptance criteria

- [ ] The Listing shows destination, departure, expected return, service fee, purchase scope, Provider, and each Errand Trip's capacity. Dated availability and pause rules use Asia/Manila.
- [ ] A Buyer can request a trip through the shared Order Request and conversation flow. Submission reserves no capacity.
- [ ] Confirmation atomically commits trip capacity and freezes the agreed scope, fee, schedule, and handoff.
- [ ] A cancellation cannot restore capacity to an elapsed Errand Trip; future restoration is capped at the usable committed amount.
- [ ] Tests cover separate trips, last-capacity competition, schedule visibility, and unauthorized edits.

## Comments
