# 18: Offer Food Batches

Status: ready-for-agent
Blocked by: 13 Confirm and cancel Transactions

## What to build

A Seller publishes a reusable Food & Drinks Listing with a dated Food Batch. Buyers can discover the batch, request it, and receive a confirmed Transaction against its remaining quantity.

## Acceptance criteria

- [ ] The Listing shows food or drink name, description, price, availability, handoff, Seller, and a dated Food Batch with quantity and fulfillment window.
- [ ] A ready-to-order Food Batch works without enabling pre-orders. Its Available Now state follows the window, pause, and remaining quantity.
- [ ] Buyers can request a batch; submission reserves nothing, while confirmation atomically commits its quantity.
- [ ] Cancelling restores only quantity still usable before the Food Batch expires; completion restores none.
- [ ] Tests cover batch-specific quantity, competing confirmations, and no cross-batch stock leakage.

## Comments
