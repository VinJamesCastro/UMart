# 27: Send best-effort web push

Status: ready-for-agent
Blocked by: 09 Message from a Listing, 10 Submit a Marketplace Order Request, 11 Discuss, decline, or cancel a request, 13 Confirm and cancel Transactions

## What to build

A Member can opt into web push for new requests, Seller or Provider confirmations, cancellations, and new messages. The in-app notice and visible deadline remain useful when push cannot arrive.

## Acceptance criteria

- [ ] In-app notices cover request, message, Transaction, review, Listing, support, and report events where appropriate and while their records are retained. Push subscription requires Member permission and a supporting browser; refusal or delivery failure leaves in-app notices and deadlines intact.
- [ ] Supported iOS users see Home Screen installation guidance before the app requests push permission.
- [ ] Push is sent for the four pilot event types and contains no message body, private deal details, or price.
- [ ] Public Listing title and sender username may appear only after stripping phone numbers and exact room patterns.
- [ ] Tests inspect generated payloads and the in-app fallback; push delivery is treated as best effort.

## Comments
