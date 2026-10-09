# 02: Guest Live Listing discovery

Status: ready-for-agent
Blocked by: None (can start immediately)

## What to build

A guest opens the mobile-friendly UHome Community Marketplace and sees a seeded Live Marketplace Listing without signing in. This first path establishes the running website, public Listing data, and the pilot's application-level test seam.

## Acceptance criteria

- [ ] The public Listing detail shows title, description, photos, price, category, availability, and Seller username on a phone-sized viewport.
- [ ] Draft, Held, rejected, and removed Listings are absent from guest discovery. A Live Listing can be viewed even when it is unavailable for requests.
- [ ] Guest data access does not expose optional floor, Google identity, private profile details, messages, requests, or Transactions. Direct Supabase reads are checked as well as the page.
- [ ] The site calls participants UMart Members and makes no residency-verification claim.
- [ ] A running-app test covers the guest path against an isolated Supabase environment.

## Comments
