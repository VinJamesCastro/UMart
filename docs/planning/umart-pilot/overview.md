# UHome UMart pilot planning overview

This file is the planning overview. The implementable work is in tickets 02–29 below; ticket numbers were kept so their existing dependency references stay valid. Start with ticket 02, then work on tickets whose **Blocked by** requirements are complete.

Implement the confirmed UHome pilot described in the [product requirements](PRODUCT.md) and [build spec](spec.md). The spec covers guest Listing discovery, member identity and privacy, all four Listing categories, availability, Order Requests, Transactions, messaging, ratings, moderation, support, notices, and pilot reporting. Preserve the domain terms and ADR decisions referenced there.

Implementation is split into coherent, independently verifiable tickets. Use the spec's testing decisions as the acceptance boundary, including direct checks of private data authorization.

## Foundation and Marketplace

- [02 Guest Live Listing discovery](issues/02-guest-live-listing-discovery.md)
- [03 UMart Member sign-in and profiles](issues/03-member-sign-in-and-profiles.md)
- [04 Publish a Marketplace item](issues/04-publish-marketplace-item.md)
- [05 Review keyword-held Listings](issues/05-review-keyword-held-listings.md)
- [06 Marketplace availability](issues/06-marketplace-availability.md)
- [07 Browse Home and Explore](issues/07-browse-home-and-explore.md)
- [08 Save Listings privately](issues/08-save-listings-privately.md)

## Requests and Transactions

- [09 Message from a Listing](issues/09-message-from-listing.md)
- [10 Submit a Marketplace Order Request](issues/10-submit-marketplace-order-request.md)
- [11 Discuss, decline, or cancel a request](issues/11-discuss-decline-or-cancel-request.md)
- [12 Expire and erase Order Requests](issues/12-expire-and-erase-order-requests.md)
- [13 Confirm and cancel Transactions](issues/13-confirm-and-cancel-transactions.md)
- [14 Claim and confirm fulfillment](issues/14-claim-and-confirm-fulfillment.md)
- [15 Auto-confirm unanswered claims](issues/15-auto-confirm-unanswered-claims.md)
- [16 Resolve disputed fulfillment](issues/16-resolve-disputed-fulfillment.md)
- [17 Publish transaction-linked reputation](issues/17-publish-transaction-linked-reputation.md)

## Categories and discovery

- [18 Offer Food Batches](issues/18-offer-food-batches.md)
- [19 Open food pre-orders](issues/19-open-food-preorders.md)
- [20 Offer Service Slots](issues/20-offer-service-slots.md)
- [21 Offer Errand Trips](issues/21-offer-errand-trips.md)
- [22 Filter all four categories](issues/22-filter-all-four-categories.md)

## Trust, support, and launch

- [23 Report Members and activity](issues/23-report-members-and-activity.md)
- [24 Block another Member](issues/24-block-another-member.md)
- [25 Provide onboarding and FAQ](issues/25-provide-onboarding-and-faq.md)
- [26 Handle support issues](issues/26-handle-support-issues.md)
- [27 Send best-effort web push](issues/27-send-best-effort-web-push.md)
- [28 Report pilot measures](issues/28-report-pilot-measures.md)
- [29 Prepare the hosted pilot](issues/29-prepare-hosted-pilot.md)
