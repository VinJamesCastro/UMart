# 03: UMart Member sign-in and profiles

Status: ready-for-agent
Blocked by: 02 Guest Live Listing discovery

## What to build

A person signs in with Google, chooses a public username, and becomes a UMart Member. Signed-in Members can view full profiles and an optional self-reported UHome floor without revealing Google account details to other Members.

## Acceptance criteria

- [ ] Google sign-in creates one account usable as Buyer, Seller, or Provider; no residency verification is implied.
- [ ] The Member can set a public username and About description and optionally select a self-reported floor from UHome's 38 floors. Signup and profile have no room-number field.
- [ ] Guests cannot view full profiles or floor. Other Members cannot read the account's Google email or profile identity.
- [ ] Profile and account data permissions are enforced by Supabase policies, with cross-account read and write tests.
- [ ] The sign-in flow works at a phone-sized viewport and returns the Member to the action that required sign-in.

## Comments
