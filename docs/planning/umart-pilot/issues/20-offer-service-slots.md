# 20: Offer Service Slots

Status: ready-for-agent
Blocked by: 13 Confirm and cancel Transactions

## What to build

A Provider publishes a reusable service Listing with dated Service Slots. A Buyer can request a slot, discuss scope, and receive a confirmed Transaction against its capacity.

## Acceptance criteria

- [ ] The Listing shows service description, price or rate, availability, Provider, and each Service Slot's time and capacity. Applicable recurring or dated availability and pause rules use Asia/Manila.
- [ ] Buyers can request a Service Slot through the shared Order Request and conversation flow; submission reserves no capacity.
- [ ] Confirmation atomically commits the selected slot's capacity and freezes scope, price, schedule, and handoff.
- [ ] Cancelling an elapsed Service Slot cannot restore its capacity. A future cancellation restores no more than the usable committed amount.
- [ ] Tests cover distinct slots, competing confirmations, elapsed cancellation, and unauthorized edits.

## Comments
