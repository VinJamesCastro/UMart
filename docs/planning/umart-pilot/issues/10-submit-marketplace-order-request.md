# 10: Submit a Marketplace Order Request

Status: ready-for-agent
Blocked by: 06 Marketplace availability

## What to build

A Buyer submits one Order Request for an available Marketplace Listing. Both participants see a Pending Request, and the Seller receives an in-app notice and response deadline.

## Acceptance criteria

- [ ] The request concerns one Listing and can ask for multiple units, a proposed time, and a handoff arrangement. There is no cart.
- [ ] Submission snapshots the Listing title, offered price, requested quantity, proposed time and handoff, and both participants. Later Listing edits do not change the snapshot.
- [ ] Submission does not reserve stock or guarantee fulfillment, and the interface says so. Unavailable Listings reject new requests.
- [ ] The ordinary Pending Request deadline is the earlier of 24 hours after submission or proposed fulfillment start, displayed to both parties.
- [ ] Only the Buyer and Seller can read the request; the Seller gets an in-app notice. Tests cover snapshot stability, no reservation, and denied cross-account access.

## Comments
