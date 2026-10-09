# 09: Message from a Listing

Status: ready-for-agent
Blocked by: 03 UMart Member sign-in and profiles, 04 Publish a Marketplace item

## What to build

A Buyer and Seller start a private conversation from a Listing without exchanging personal social accounts.

## Acceptance criteria

- [ ] A signed-in Member can send and receive Listing-level messages with the Listing's author; a guest is prompted to sign in.
- [ ] Only the participants can read or write the conversation. Direct Supabase access by another Member is denied.
- [ ] New messages create an in-app notice, and the Inbox shows the conversation.
- [ ] This separate Listing conversation is not tied to an Order Request's later erasure.
- [ ] A running-app test covers two participants and a third Member who cannot inspect the conversation.

## Comments
