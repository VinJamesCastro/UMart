# 11: Discuss, decline, or cancel a request

Status: ready-for-agent
Blocked by: 09 Message from a Listing, 10 Submit a Marketplace Order Request

## What to build

Before confirmation, the Buyer and Seller can discuss an Order Request. The Seller can mark it Discussing or decline it, and either participant can cancel it with a reason.

## Acceptance criteria

- [ ] The participants can exchange private request-linked messages; the Listing conversation remains separate.
- [ ] Marking a Pending Request Discussing satisfies its initial response deadline without reserving stock or promising fulfillment.
- [ ] The displayed Discussing deadline is proposed fulfillment start or, if no start exists, seven days after the last message.
- [ ] Decline and unconfirmed cancellation stop the request and notify the other participant; cancellation records a reason. The Seller manually declines each pending request they cannot fulfill.
- [ ] Tests cover the allowed actors, state transitions, notices, and unchanged request snapshot.

## Comments
