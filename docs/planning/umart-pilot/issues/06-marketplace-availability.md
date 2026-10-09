# 06: Marketplace availability

Status: ready-for-agent
Blocked by: 04 Publish a Marketplace item

## What to build

A Seller sets when a Marketplace item is available and can pause it. A Buyer sees its actual request state, while a Live Listing remains browseable when unavailable.

## Acceptance criteria

- [ ] The Seller can set recurring, specific-date, one-time, or until-sold-out availability where applicable, and can pause or resume the Listing.
- [ ] All displayed and evaluated times use Asia/Manila. Available Now appears only inside an open window with stock remaining and no pause.
- [ ] Not-yet-open, paused, sold-out, and other unavailable Live Listings remain visible with no new request action.
- [ ] Publication and availability remain separate; changing availability does not publish a draft or hide a Live Listing from guest browsing.
- [ ] Tests exercise opening and closing boundaries, pause, and zero stock under a controlled clock.

## Comments
