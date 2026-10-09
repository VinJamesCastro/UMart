# 19: Open food pre-orders

Status: ready-for-agent
Blocked by: 12 Expire and erase Order Requests, 18 Offer Food Batches

## What to build

A Seller can enable pre-ordering for a future Food Batch. Buyers see its request window and Seller response deadline before asking for it.

## Acceptance criteria

- [ ] The Seller sets opening, request cutoff, fulfillment date or window, batch quantity, and a response deadline after cutoff and no later than fulfillment start.
- [ ] Pre-order Open appears only while the request window is open. Requests outside the window are rejected.
- [ ] The Buyer sees the response deadline before submission. It replaces the ordinary 24-hour Pending Request deadline for this window.
- [ ] Submission does not reserve stock. The Seller may confirm pending requests in any order, with capacity committed only on confirmation.
- [ ] Controlled-time tests cover opening, cutoff, response expiry, and competing confirmations.

## Comments
