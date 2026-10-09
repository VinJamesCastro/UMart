# UMart — Product Requirements

## 1. Product Summary

**UMart** is a **UHome Community Marketplace** for discovering goods, food and drinks, services, and errands offered around UHome. It is designed for the UHome community, but pilot accounts do not verify residency and public listings are visible to anyone with the link.

It gives members one place to discover and interact with people offering:

- Used and pre-loved items
- Food and drinks
- Services
- Errands and pasabuy
- Other community-based products or offerings

UMart is initially being tested within **UHome / University Home**. UHome will serve as the first community, but the product is designed so the same platform can eventually support other dorms, residences, condos, and university communities.

The initial release is a mobile-friendly website shared through the UHome group chat. Members can optionally add it to their phone's home screen. UMart is free to use during the pilot; initial hosting aims to stay within free-service limits.

### Core value proposition

For buyers:
> Find useful products, food, services, and errands offered around UHome.

For sellers/providers:
> Offer products or services to UMart Members around UHome without repeatedly posting in a group or having to expose personal social-media accounts.

For the community:
> Have one organized place to discover what people nearby are offering.

---

## 2. Product Vision

UMart should feel like a **small, community-specific version of a marketplace/social platform**, rather than a full-scale food-delivery company.

The product combines:

**Community discovery + Marketplace + Messaging + Order Requests**

The central product idea is:

> **People around UHome can discover offers, communicate privately, and organize transactions without needing to exchange personal social accounts.**

UMart is not intended to become a general-purpose social network, payment processor, or delivery company.

---

## 3. Initial Community: UHome

### UHome MVP

The first version of UMart will be shared with the **UHome community**. The pilot does not establish that every account belongs to a tenant.

UHome currently has **38 floors**.

The community structure should support:

```text
UMart
└── UHome
    ├── Floor 1
    ├── Floor 2
    ├── Floor 3
    ├── ...
    └── Floor 38
```

The application should ultimately support multiple communities, but the MVP should primarily optimize for the UHome use case.

---

## 4. User Identity & Privacy

UMart should use a **public username / private account information** model. A signed-in participant is a **UMart Member**, not a verified resident.

### Member profile

Full profiles are visible to signed-in members. Example:

```text
@Mika
UMart Member
30th Floor, if the member chooses to provide it
```

Users do **not** need to expose their:

- Facebook account
- Instagram account
- Personal social profiles
- Phone number
- Other personal contact information

### Floor and room details

Floor is optional and self-reported. A member must sign in to see another member's floor. UMart does not ask for an exact room number at signup and has no room field in the pilot profile. Members may share a room number or another meeting point in private messages when coordinating a transaction.

Possible pickup locations include:

- UHome lobby
- Common area
- A mutually agreed floor/location
- A user's room, only if both parties voluntarily agree

### Important privacy principle

UMart recommends sharing exact room numbers, phone numbers, social contacts, and meeting details in private messages. A seller may choose to include their own contact or room details in a public listing. Listing text and photos are visible to anyone with the link, so onboarding and the FAQ must explain that exposure. Listings may not reveal another person's private information.

---

## 5. Community Access & Verification

UMart is intended to be community-based, but the MVP does **not** depend on UHome administration or an official partnership with UHome.

This is intentional because requiring administrators to manually verify users or perform ongoing work would create an unnecessary dependency during early testing.

### MVP approach

The initial launch link will be shared in the UHome community group chat. Anyone with that link may browse public listings before signing in. Public listing information includes the title, description, photos, price or rate, category, availability, and seller's or provider's public username. A forwarded link may reach someone outside UHome.

Google sign-in is required to see full profiles or optional floor details, save listings, submit requests, send messages, post listings, rate members, or report issues. Sign-in does not verify residency. UMart does not add a residency check during the pilot. The product should say **UHome Community Marketplace** and label participants **UMart Members**.

The Google account identifies the member privately; their UMart username is displayed publicly. Their Google profile and email address are not displayed to other members.

### Verification status

UMart should **not claim “Verified UHome Resident”** unless there is an actual verification process behind that label.

A stronger verification system can be introduced later if UMart expands and gains formal partnerships or a reliable way to verify residency.

---

## 6. Core Marketplace Categories

### 6.1 Marketplace

In the navigation, **Marketplace** is the category for physical items. UMart as a whole includes Marketplace, Food & Drinks, Services, and Errands / Pasabuy. Members can list new or used items. A one-off item's stock lives on its Listing.

Examples:

- Furniture
- Electronics
- Appliances
- Clothes
- Dorm supplies
- School supplies
- Decorations
- Other personal belongings

A Marketplace item listing should support:

- Photos
- Title
- Description
- Price
- Condition
- Availability
- Pickup/delivery method
- Seller
- Optional floor, visible to signed-in members

---

### 6.2 Food & Drinks

Members can sell food and beverages directly to other members. A reusable food Listing can have dated **Food Batches**, each with its own quantity and fulfillment window.

Examples:

- Matcha
- Coffee
- Meals
- Snacks
- Desserts
- Homemade food

Food listings/products should support:

- Product name
- Description
- Price
- Quantity per Food Batch
- Availability
- Pre-order settings
- Pickup/delivery method
- Seller
- Optional floor, visible to signed-in members

---

### 6.3 Services

Members can offer services to other members. A reusable service Listing can have dated **Service Slots**, each with capacity for that time window.

Examples:

- Tutoring
- Printing
- Laundry
- Haircuts
- Repairs
- Graphic design
- Photography
- Tech assistance
- Other useful member-to-member services

A service listing should support:

- Service description
- Price or rate
- Availability
- Capacity per Service Slot
- Provider
- Optional floor, visible to signed-in members
- Request/contact flow

---

### 6.4 Errands / Pasabuy

Members can offer to perform errands for other members. A reusable errand Listing can have dated **Errand Trips**, each with its own capacity.

Examples:

> Going to SM at 6 PM. Anyone needs pasabuy?

> Going to Puregold. Can buy groceries for people nearby.

An errand listing should support:

- Destination
- Departure time
- Expected return time
- Service fee
- Capacity/available slots
- What the provider is willing to purchase
- Request flow

All four categories appear at launch. A category with no real Listings shows a clear empty state and invites the first member to post.

---

## 7. Product Availability

Availability is a core UMart concept, particularly for food, drinks, services, and errands.

Sellers/providers should be able to define:

All displayed and evaluated times use **Philippine time (Asia/Manila)**. A seller can pause an offering at any time.

### Recurring availability

Example:

```text
Monday–Friday
6:00 PM–10:00 PM
```

### Specific-date availability

Example:

```text
October 5
6:00 PM–9:00 PM
```

### One-time availability

Example:

```text
Today only
6:00 PM–9:00 PM
```

### Until sold out

Example:

```text
10 items available
```

Paused, sold-out, not-yet-open, and one-off unavailable Listings stay browseable with a clear state and no new request action. Existing confirmed Transactions remain accessible to their participants. The goal is for members to understand what is actually available instead of seeing outdated community posts.

Keep a Listing's publication state separate from its availability. Publication can be draft, held for review, live, rejected, or removed. A live Listing can still be paused, not yet open, sold out, or otherwise unavailable. Only live Listings are browseable by guests.

---

## 8. Pre-Ordering

**Pre-ordering is a seller-controlled option for food and drink products.** A seller can offer ready-to-order products without enabling pre-orders.

Example:

```text
Strawberry Matcha
₱140

Pre-order for October 5
Orders open: 10:00 AM
Orders close: 4:00 PM
Pickup: 6:00–8:00 PM
Stock: 20
```

Pre-ordering should support use cases such as:

- Next-day menus
- Limited batches
- Weekend batches
- Scheduled preparation
- Products that need to be ordered before a specific cutoff time

When enabled, a pre-order has an opening time, request cutoff, fulfillment date or window, and Food Batch quantity. Buyers can submit requests while the window is open. The seller must still confirm each request; submitting one does not reserve stock or guarantee fulfillment. The seller may choose which pending requests to confirm, regardless of submission order.

The seller sets a response deadline for each pre-order window. It must fall after the request cutoff and no later than fulfillment start. Show that deadline to the buyer before they submit. This deadline replaces the ordinary 24-hour response deadline for requests in that window.

---

## 9. “Available Now” Discovery

The home experience should prioritize offerings that are currently available or becoming available soon.

**Available Now** appears only while the offering is within its availability window, has stock or capacity where applicable, and is not paused. A future batch may instead show **Pre-order Open** while its request window is open. Listings that cannot take requests show their state rather than disappearing from category discovery.

Example for a signed-in member:

```text
AVAILABLE NOW

🍵 Matcha by @Mika
₱120
30th Floor, if shared
Available until 10 PM

🍪 Cookies by @Anne
₱80
28th Floor, if shared
8 boxes remaining

🏃 Pasabuy — SM
30th Floor, if shared
Leaving at 6:30 PM
```

This is a key distinction from a conventional community feed where posts can quickly become buried or outdated.

---

## 10. Seller / Provider Profiles

Each seller/provider should have a persistent UMart profile rather than relying on repeated social-media posts.

Example:

```text
@Mika
UMart Member
30th Floor, if shared

⭐ 4.9
24 buyer-confirmed transactions

ABOUT
Matcha and drinks made to order.

LISTINGS
Classic Matcha — ₱120
Strawberry Matcha — ₱140
Dirty Matcha — ₱150
```

Signed-in members can view full profiles, including separate **seller/provider** and **buyer** rating summaries and the number of ratings behind each average. A member can have both kinds of reputation. Public completed-transaction counts include only buyer-confirmed completions.

The account owner's profile also shows their **private buying and selling history**: the item or service, other party, agreed terms, and current status. Only the transaction participants and a moderator handling a report or support issue may see these details. Other members can see public listings and ratings, but not someone's purchase history or conversations.

A UMart Member can simultaneously be a:

- Buyer
- Seller
- Service provider
- Errand provider

There should not be separate accounts for each role.

---

## 11. Listings vs. Posts

UMart may have a lightweight community/social feel, but marketplace activity should be represented as **structured listings** rather than only free-form posts.

### Example of an unstructured post

> Matcha available tonight guys. DM me.

### UMart representation

```text
Classic Matcha
₱120

Seller: @Mika
Floor: 30, visible after sign-in if shared
Stock: 10
Availability: 6 PM–10 PM
Pre-order: Available

[Request Order]
```

This structure makes information searchable, filterable, and easier to act on.

Signed-in members can save Listings as private bookmarks. Saving a Listing does not send price or availability alerts. A saved Listing that becomes unavailable or is removed stays identifiable as unavailable until the member unsaves it.

---

## 12. Messaging

UMart should include built-in messaging so users can communicate without exchanging personal social-media accounts.

Messaging should support conversations connected to a Listing or Order Request. The Buyer and Seller or Provider can discuss changes before confirmation. After confirmation, the agreed Transaction terms stay fixed; a correction requires cancellation and a new request.

Example:

```text
Buyer:
Is this still available?

Seller:
Yes. I can prepare it around 7 PM.
```

Messaging is important because UMart does **not** attempt to fully automate community transactions.

The users can discuss and agree on the practical details themselves. Request-only messages follow the Order Request retention rule. A separate Listing conversation may remain after an expired request is erased. Blocking stops new messages and requests between the two accounts.

---

## 13. Order Request Model

UMart uses one **Order Request** model for Marketplace items, food and drinks, services, and errands. A request concerns one Listing, though it may ask for more than one unit. There is no cart in the pilot. Submitting a request does not guarantee a purchase, booking, or stock reservation.

On submission, the request snapshots the Listing title, offered price or rate, requested quantity or slot, proposed time and handoff arrangement, and both participants. Later Listing edits do not silently change the request. The Seller or Provider receives a notice and sees a response deadline.

### Core flow

```text
Buyer submits Order Request → Seller or Provider receives notice
    → both discuss details; Seller or Provider may mark it Discussing
    → Seller or Provider confirms the final terms and commits capacity
    → Transaction is created; Buyer receives confirmation notice
    → parties fulfill directly; Seller or Provider claims fulfillment
    → Buyer confirms or disputes, or the response window closes
```

### Why this model is used

The Seller or Provider needs to confirm that:

- The product is actually available
- The requested quantity is possible
- The stated price is still correct
- The seller can fulfill the request
- The pickup/delivery arrangement works
- The parties have discussed the final details

This also reduces the impact of fake bookings or accidental requests.

### Deadlines and expiry

For an ordinary Pending Request, the response deadline is the earlier of 24 hours after submission or the proposed fulfillment start. A Seller or Provider can decline, confirm, or move it to **Discussing** before that deadline. Moving to Discussing satisfies the initial response deadline but does not promise fulfillment. Discussing then expires at the proposed fulfillment start; if no start time exists, it expires after seven days without a message. Food pre-orders use the seller-set response deadline described in section 8. Show the applicable deadline to both parties, especially the Seller or Provider.

When a deadline passes without confirmation, hide the Expired Order Request from normal order views immediately. Erase it with its request-only messages and notices seven days later. If an open report or moderation case needs those records, keep the necessary evidence until the case closes, then erase the request evidence. Keep only minimal moderation outcome and account-action history.

### Request and Transaction states

Before confirmation, the record is an **Order Request**:

- **Pending Request:** Buyer submitted the request. No stock or capacity is reserved.
- **Discussing:** Seller or Provider responded and the parties are clarifying terms.
- **Declined:** Seller or Provider rejected this request. They manually decline each pending request they cannot fulfill.
- **Cancelled:** Either party stopped an unconfirmed request, with a reason and notice to the other party.
- **Expired:** The applicable response or discussion deadline passed without confirmation; the request follows the erasure rule above.

When the Seller or Provider confirms, the Order Request becomes a **Transaction**. Confirmation records and freezes the final quantity or scope, price or fee, schedule, and pickup or delivery arrangement. It commits the relevant stock or capacity in the same operation. The Buyer receives a confirmation notice, but the pilot does not require a separate Buyer acceptance step. If the confirmed terms are wrong, a party can cancel with a reason and submit a corrected new request.

- **Confirmed:** The Seller or Provider confirmed the final terms; fulfillment has not been claimed.
- **Awaiting buyer confirmation:** The Seller or Provider claimed fulfillment. The Buyer can confirm or dispute it.
- **Buyer-confirmed completion:** The Buyer explicitly confirmed fulfillment. This counts as a public completion and allows each party one rating and review.
- **Auto-confirmed completion:** The Buyer did not respond within 72 hours of the fulfillment claim. It closes the Transaction subject to the seven-day late response window, but earns no public completion credit, pilot completion credit, or ratings unless the Buyer later confirms.
- **Disputed:** The Buyer contests the fulfillment claim. A moderator reviews it; public credit and ratings wait for resolution.
- **Moderator-verified completion:** A moderator upheld the fulfillment claim after a dispute. It closes the Transaction but earns no public completion credit, pilot completion credit, or ratings unless the Buyer later confirms.
- **Cancelled:** Either party ended a Confirmed Transaction with a reason and notice to the other party. A moderator may also cancel one after finding a false fulfillment claim.

After auto-confirmation, the Buyer has seven more days to confirm or dispute the claim in the Transaction. Later objections go through reporting. If a moderator finds a fulfillment claim false, remove it and return the Transaction to Confirmed if both parties still intend to proceed, or Cancelled otherwise. Record the moderation action. Both participants see current state and agreed details in their private histories and linked conversation.

For a physical item or food order, the Seller may tell the Buyer that a Confirmed order is ready for pickup. This is a fulfillment update, not a completion claim.

---

## 14. Inventory Behavior

Submitting an Order Request does not reserve stock or capacity. Marketplace one-off items use stock on the Listing. Reusable food Listings use quantity per Food Batch, service Listings use capacity per Service Slot, and errand Listings use capacity per Errand Trip. A Seller or Provider can choose which pending requests to confirm.

Confirmation must check and commit the relevant count in one operation so competing requests cannot claim the same last unit. When the last unit of a one-off Marketplace Listing is committed, its Listing becomes unavailable and stops accepting new requests. Other pending requests remain visible to their Buyers but wait for the Seller to decline each manually or for their deadlines to expire.

On cancellation of a Confirmed Transaction, the Seller or Provider chooses how much of the committed count is genuinely usable again, up to the cancelled amount. Capacity for an elapsed Service Slot or Errand Trip, or an expired Food Batch, cannot be restored. Completing a Transaction does not restore stock or capacity. If moderation cancels a falsely claimed fulfillment, apply the same usable-capacity rule.

---

## 15. Payments

UMart will **not process payments during the MVP**.

The actual payment is handled directly between the Seller or Provider and the Buyer.

Possible methods include:

- Cash
- GCash
- Maya
- Bank transfer
- Another mutually agreed method

UMart records and organizes the transaction state, but it does not act as:

- Payment processor
- Wallet
- Escrow service
- Financial intermediary

This keeps the first version focused on the actual problem: **discovery, communication, and transaction organization**.

---

## 16. Delivery & Pickup

UMart will **not operate an internal delivery fleet in the MVP**.

There will be no initial requirement for:

- Riders
- Rider dispatch
- GPS rider tracking
- Delivery fleet management
- Route optimization

Fulfillment can happen through:

### Pickup

The Buyer collects the item or order from an agreed location.

### Seller delivery

The seller/provider delivers personally when they choose to.

### Community errands

Another UMart member can fulfill the request through an errand/pasabuy listing.

---

## 17. Ratings & Reputation

Only after the **Buyer explicitly confirms completion** can each party optionally leave one rating and review for the other party:

- **Buyer rates seller/provider** for the offering and their experience. The review appears on the seller/provider's public profile.
- **Seller/provider rates buyer** for their experience, such as communication and following the agreed arrangement. The review appears on the buyer's public profile.

Reviews must be linked to a Buyer-confirmed Transaction and show whether the author was the Buyer or Seller/Provider. Public reviews should not reveal room numbers, contact information, private order details, or conversation messages. A seller fulfillment claim, auto-confirmation, moderator-verified completion, or unresolved dispute does not unlock reviews. The moderator can remove abusive reviews or ratings associated with a fabricated Transaction.

Example:

```text
⭐ 5.0
Fast response and good matcha.
```

Profiles can show:

- Buyer-confirmed completed Transactions by role
- Separate buyer and seller rating averages and rating counts
- Buyer and seller review history

Buyer and seller ratings are counted separately and only come from **Buyer-confirmed completed Transactions**.

---

## 18. Safety & Moderation

The pilot must publish short community Listing rules before members post. The rules shown to members are:

> UMart is made for useful, honest, community-based offers. Before posting a listing, please make sure your offer is clear, accurate, and safe for other users.
>
> Listings should describe the actual product, service, errand, or offer. Include the correct price or rate, quantity or capacity, availability, and handoff details.
>
> Do not use misleading photos, fake details, or impersonate another person.
>
> UMart does not allow listings involving:
>
> - Stolen or counterfeit goods
> - Weapons or dangerous items
> - Controlled substances or illegal drugs
> - Alcohol, tobacco, or vapes
> - Gambling offers
> - Sexual services
> - Selling accounts, IDs, or identity documents
> - Harassment, spam, threats, or scam behavior
>
> Listings must not expose another person's private information.
>
> Sellers may choose to include their own contact details or room details in a public listing, but UMart recommends sharing exact room numbers, phone numbers, social media accounts, or meeting details through private messages instead.
>
> UMart does not verify food safety, preparation methods, or kitchen conditions. Buyers and sellers are responsible for discussing details before completing a transaction.
>
> Every exact match on the founder-approved prohibited keyword list is held for founder/admin review before publication. A match does not automatically reject the listing. The founder/admin may approve a false positive, reject a prohibited listing, or ask the author to edit and resubmit.
>
> Reports and less certain warning signs go to the review queue, but they do not automatically hide a live listing unless the founder/admin decides action is needed.
>
> If a listing is rejected or removed, the author sees the reason and may edit and resubmit it when appropriate.

Normal Listings appear immediately. Repeated reports and suspicious patterns also enter the review queue without automatically hiding a live Listing. The founder/admin may approve, reject, or remove unsafe, illegal, misleading, or inappropriate offers. A held or rejected author sees the Listing's status and reason and can edit and resubmit when appropriate.

Users should be able to:

- Report a listing
- Report a user
- Report a transaction
- Block a user

A UMart moderator/admin should be able to:

- Review reports
- Remove listings
- Suspend users
- Take action against problematic activity

Blocking stops new direct messages and requests between the two members and hides the blocked member from the blocker's signed-in views. Public Listings may still be visible to a guest. A previously Confirmed Transaction stays visible to its participants with cancel and report actions, but no new direct contact; a moderator can help if needed.

Safety features should be simple enough for the pilot but should exist from the beginning because UMart facilitates interactions involving money, food, and physical meetups.

---

## 19. Notifications

UMart launches with in-app notices and best-effort web push. In-app notices are the reliable place to check marketplace, messaging, order, and support events while those records are retained. Web push covers new requests, Seller or Provider confirmations, cancellations, and new messages. Members must grant permission and use a browser that supports push; push delivery cannot be guaranteed. On iOS, members need to add the web app to the Home Screen before it can request push permission. Response deadlines remain clearly visible inside the app.

Examples:

- New order request
- New message
- Order request declined
- Order confirmed
- Order marked for discussion
- Order ready
- Order cancelled
- Seller or Provider claimed fulfillment
- Buyer confirmed or disputed fulfillment
- New buyer or seller review
- Listing sold/completed
- Support ticket update
- Report status update, when appropriate

Push text may include the public Listing title and sender's public username. It must strip phone numbers and exact room patterns and omit message bodies, private deal details, and prices. The pilot does not need an elaborate notification-preferences system.

---

## 20. Onboarding

UMart should include a short first-time onboarding flow so new users understand how the app works before using the marketplace.

The onboarding should be brief, visual, and focused on the concepts a user needs to understand immediately.

### Core onboarding topics

1. **What is UMart?**
   - A UHome Community Marketplace designed around UHome offers. Having an account does not verify residency.

2. **What can you do?**
   - Buy and sell items
   - Order food and drinks
   - Offer services
   - Offer or request errands/pasabuy

3. **How does privacy work?**
   - Users have a UMart username
   - Listing text and photos are visible to anyone with the link
   - Their optional floor is visible to signed-in members
   - There is no room field at signup; exact room and contact details are best shared in private messages
   - Personal social-media accounts do not need to be shared

4. **How do order requests work?**
   - A Buyer submits a request and sees its response deadline
   - The Seller or Provider receives a notice and can discuss details
   - Seller or Provider confirmation freezes the agreed terms and notifies the Buyer
   - Seller or Provider claims fulfillment; the Buyer confirms or disputes it
   - Payment and fulfillment happen directly between the parties

If a member wants web push on iOS, onboarding and the FAQ should explain how to add UMart to the Home Screen and grant notification permission. In-app notices and visible deadlines remain available without push.

5. **How should the community be used?**
   - Be respectful
   - Provide accurate listing information
   - Follow UMart community rules
   - Report suspicious, abusive, or prohibited activity

Users should be able to revisit onboarding/help information later through the Help/FAQ area. The essential privacy and safety information should remain accessible even after onboarding is completed.

---

## 21. Help, FAQ & User Support

UMart should include an in-app **Help / FAQ** area so users can quickly understand common workflows and solve common problems without needing a moderator for every question.

### FAQ areas

The FAQ should cover practical questions such as:

- What is UMart?
- Who can use UMart?
- How do I access the UHome community?
- How do I create a listing?
- How do I sell an item?
- How do I sell food or drinks?
- How do I offer a service?
- How do I create a pasabuy/errand listing?
- How do I place an order request?
- What happens after I submit an order request?
- When does a request expire, and what happens to its messages?
- How does seller confirmation work?
- What counts as a completed Transaction for ratings and public counts?
- How does pre-ordering work?
- How do availability schedules work?
- Does UMart process payments?
- How are payments handled?
- How do pickup and delivery work?
- Can other users see my room number?
- Who can see my Listing or profile, and does UMart verify residency?
- How do saved Listings and blocking work?
- Why might a push notice not arrive?
- How do messaging and order conversations work?
- How do ratings and reviews work?
- What should I do if a Seller, Provider, or Buyer does not respond?
- How do I report a member or listing?
- What should I do if I encounter suspicious or unsafe behavior?

The FAQ should explain actual UMart behavior and rules using simple language.

### Report an issue / Get help

Users should be able to submit a support issue when they encounter a technical problem, account issue, marketplace problem, or another issue that the FAQ cannot resolve.

A support form should allow the user to provide:

- Issue category
- Short summary
- Detailed description
- Related listing, member, or order, when applicable
- Screenshots or other supporting evidence, when applicable

Possible categories include:

- Technical issue
- Account/profile issue
- Listing issue
- Order/request issue
- Messaging issue
- Safety concern
- Payment-related concern
- Other

For payment-related concerns, UMart can review reported conduct under its community rules. It does not decide who owes money, issue refunds, or act as the payment intermediary; payment remains between Buyer and Seller or Provider.

Support requests should have a status such as:

- Open
- Under review
- Resolved
- Closed

---

## 22. Reporting Members, Listings & Transactions

UMart should provide a dedicated reporting system for problematic activity.

Users should be able to report:

- A member
- A listing
- An order/transaction
- A message or conversation, when applicable

### Report Member flow

A user selects **Report Member**, chooses a reason, and can provide supporting context and evidence.

Possible reasons include:

- Scam or fraud concern
- Harassment or inappropriate behavior
- Fake or misleading identity
- Prohibited item or service
- Suspicious activity
- Spam
- Repeated rule violations
- Other

The report should allow the user to provide:

- Written explanation
- Screenshots
- Photos or other evidence
- Related listing
- Related order
- Related conversation/message

Evidence should be attached to the report so moderators can review the situation rather than relying only on the reporter's description.

### Report Listing flow

Users can report a listing for reasons such as:

- Misleading information
- Prohibited item/service
- Suspicious/scam-related listing
- Spam
- Inappropriate content
- Other rule violation

### Report Transaction / Conversation flow

Users can also report an order, transaction, or conversation when the issue is specifically related to an ongoing or completed interaction.

An Expired Order Request and its request-only evidence are erased seven days after expiry unless a report or moderation case is open. Preserve only the evidence needed while the case is open. After resolution, erase the request evidence and retain minimal outcome and account-action history.

### Moderation

Reports should be stored in a moderator queue with a status and history.

A moderator can review the submitted information and take an appropriate action under UMart's community rules.

Possible outcomes include:

- No action
- Warning
- Remove listing/content
- Restrict account activity
- Suspend account
- Other moderation action

A report should **not automatically assume the reported allegation is true**. The purpose of the evidence and review process is to give moderators enough context to make an informed moderation decision.

For a Disputed Transaction, the founder/admin decides whether the fulfillment claim stands. If false, remove the claim and return the Transaction to Confirmed if both parties continue, or Cancelled otherwise; restore only capacity the Seller or Provider can use again. If fulfillment is upheld, close it as moderator-verified completion, with no public completion credit or ratings unless the Buyer later confirms.

---

## 23. Community / Social Layer

UMart can have a lightweight community-feed feeling similar to Facebook, but only within the context of community commerce.

The **Home feed** shows Listings from all four UMart categories together: Food & Drinks, Marketplace, Services, and Errands / Pasabuy. It is a general view of community offerings, while each Listing remains a structured item that can be searched and filtered. Guests can browse public Listings. Signed-in members can request them when available.

Users should be able to discover:

- New listings
- Food and drinks
- Services
- Errands
- Sellers/providers
- Popular or active offerings
- Available-now offerings

UMart should **not** become a general-purpose social network.

The social layer exists to improve discovery and communication around marketplace activity.

---

## 24. Initial Navigation

The initial application can use five primary areas:

### Home

General feed of offerings across all four categories, with clear **Available Now**, **Pre-order Open**, and unavailable states. Show four visible category shortcuts: **Food & Drinks**, **Marketplace**, **Services**, and **Errands / Pasabuy**. Tapping one opens Explore with that category already selected. Category discovery should use visible controls rather than requiring a user to swipe through category pages.

### Explore

Search and category browsing. The selected category determines which filters and sorting choices appear:

| Category | Filters | Sorting |
| --- | --- | --- |
| Food & Drinks | Drinks, meals, snacks, desserts; available now or pre-order; price range | Newest or price |
| Marketplace | Furniture, electronics, appliances, clothes, and other items; condition; price range | Newest or price |
| Services | Service type; availability; price range | Newest or price |
| Errands / Pasabuy | No subcategory filters required initially | No category-specific sorting required initially |

Choosing a type such as **Furniture** filters which listings are shown; choosing **Price: Low to High** sorts their order. Search can work across all categories or within the one currently selected.

An empty category shows a clear empty state and invites a member to post its first Listing. Unavailable or removed Listings saved by a member remain identifiable in their private bookmarks until unsaved.

### Orders

Private buying and selling history, including Pending, Discussing, Declined, Expired, Confirmed, Awaiting buyer confirmation, Buyer-confirmed, Auto-confirmed, Disputed, Moderator-verified, and Cancelled states where applicable.

### Inbox

Buyer/seller conversations.

### Profile

User profile, public buyer and seller ratings, Listings, availability, private saved Listings and buying/selling history for the account owner, and account/help access. Full profiles and optional floors require sign-in.

---

## 25. Initial User Types

### Buyer

Can:

- Browse
- Search
- View listings
- Save Listings privately
- Message sellers/providers
- Submit order requests
- Request services/errands
- Complete transactions
- Confirm or dispute fulfillment and review Buyer-confirmed Transactions
- View their private buying history and buyer rating

### Seller / Provider

Can:

- Create listings
- Create food/drink products
- Create services
- Set price
- Set availability
- Set stock
- Receive notifications
- Message Buyers
- Discuss, confirm, or decline requests
- Confirm transactions
- Claim fulfillment of Confirmed Transactions
- Optionally review Buyers after they confirm completion
- View their private selling history and seller rating

### Errand Provider

Can:

- Create an errand/pasabuy listing
- Set destination
- Set schedule
- Set service fee
- Confirm or decline requests
- Communicate with requesters
- Complete requests

These are not separate account types. A single UMart member can perform all of these activities.

### Moderator / Admin

Can:

- Review reports
- Review support requests
- Review held Listings and approve, reject, or request edits
- Resolve disputed fulfillment claims
- Remove listings/content
- Suspend or restrict accounts
- Moderate the community

---

## 26. MVP Scope

### Must Have

- UHome community
- UHome group-chat link distribution, without a claim of verified residency
- Guest browsing of public Listing fields
- User accounts
- Google sign-in for full profiles and participation
- Public username and UMart Member identity
- Optional, self-reported floor visible to signed-in members; no signup room field
- User profiles
- Marketplace item listings
- Food & drink listings
- Service listings
- Errand/pasabuy listings
- Search
- Categories
- General Home feed with visible category shortcuts and category-specific Explore filters and sorting
- Availability schedules
- Stock/quantity
- Food Batches, Service Slots, and Errand Trips with dated stock or capacity
- Optional seller-enabled pre-ordering for food and drinks
- Available-now discovery
- Listing details
- In-app messaging
- Private saved Listings
- Order requests
- One Listing per request, request snapshots, visible response and discussion deadlines, expiry, and erasure
- Seller notification for order requests
- Buyer and Seller or Provider conversation flow
- Seller confirmation flow
- Frozen confirmed Transaction terms and stock/capacity commitment
- Transaction states for fulfillment claims, Buyer confirmation, auto-confirmation, disputes, and moderator resolution
- Optional, transaction-linked ratings/reviews in both directions after Buyer-confirmed completion
- Separate public buyer and seller ratings, with private buying and selling history
- Report member/listing/transaction functionality
- Evidence attachments for reports
- Basic moderation tools
- Published Listing rules, exact-match keyword holds, and author status/reason with edit and resubmit
- Member blocking
- FAQ/help center
- User support / issue reporting
- Basic onboarding
- In-app notices and best-effort web push for new requests, confirmations, cancellations, and messages
- Mobile-friendly website shared through the UHome group chat, with Google sign-in

### Explicitly Not Required for MVP

- UMart payment processing
- UMart wallet
- Escrow
- Refund/payment-dispute infrastructure
- Internal delivery fleet
- Rider accounts
- Live rider tracking
- Route optimization
- Official UHome administration integration
- Complex resident-verification partnerships
- AI recommendations
- AI marketplace assistant
- Advanced seller analytics
- Full social-network functionality
- Advanced community-management infrastructure beyond what is needed for UHome testing

---

## 27. Product Principles

### 1. Community-first

UMart is built around offers relevant to the UHome community.

### 2. Privacy by default

Users should be able to transact without exposing personal social-media accounts or exact room information publicly.

### 3. Structured commerce

UMart should turn informal community posts into useful, searchable listings with price, stock, availability, and ordering information.

### 4. Human confirmation

UMart organizes the request and Transaction, but the Buyer and Seller or Provider remain responsible for discussing the final deal. The Seller or Provider confirms and records its terms.

### 5. No unnecessary middleman

Payments and physical fulfillment remain between the parties during the MVP.

### 6. Community accountability

Users can report problematic behavior and provide evidence, while moderators review reports before taking action.

### 7. Small first

UHome is the first real-world test. Features should be built to solve UHome's actual problems before expanding into a broader platform.

---

## 28. The Core User Experience

The target experience is:

> Open UMart → find an offer around UHome → sign in to request it → discuss the details → Seller or Provider confirms the Transaction → complete the handoff → Buyer confirms fulfillment → return for another useful offer.

The product should make this easier than searching through scattered community posts.

---

## 29. Product Differentiation

UMart should not compete with Facebook by trying to become a larger social network.

Its value comes from making community commerce **structured and discoverable**.

### Existing community-post experience

> “Matcha available tonight guys. DM me.”

### UMart experience

```text
Classic Matcha
₱120

@Mika
UMart Member
30th Floor, visible to signed-in members if shared

10 available
6 PM–10 PM
Pre-order available

[Request Order]
```

The goal is not to remove the human conversation. The goal is to make the conversation happen **around an organized listing and transaction**.

---

## 30. Product Success Question

The UHome pilot asks whether people use UMart for the full transaction flow and return to use it again instead of relying only on the group chat. Look for structured Listings, offer discovery, submitted Order Requests, coordination through messages, completed Transactions, and repeat buying. All four categories launch, but the pilot succeeds or fails overall rather than requiring a completed Transaction in each category.

Measure the first four weeks after the UHome group-chat link is shared against these targets:

- At least **20 Buyer-confirmed Transactions**.
- At least **10 distinct Buyers** with a Buyer-confirmed Transaction.
- At least **5 Buyers** who return for another Buyer-confirmed Transaction.

Exclude founder/test activity and self-transactions from those targets. Track Auto-confirmed and moderator-verified outcomes separately. Report counts of users (accounts), Listings, Order Requests, and Buyer-confirmed Transactions overall and by category. Do not describe accounts as verified UHome tenants.

---

## 31. Initial Build & Operating Cost

UMart should be free for members to use at launch. Aim to keep initial hosting at **₱0** while remaining within free-service limits; this is an operating target, not a promise that unlimited usage is free.

- **Website:** A mobile-friendly site hosted on Cloudflare Pages using its provided `pages.dev` address, so an initial custom domain is unnecessary.
- **Application data and accounts:** Supabase Free for Google sign-in, profiles, listings, messages, requests, reviews, and reports. Enforce authorization on data so only the appropriate users and moderator can access private records.
- **Images and evidence:** Start with free storage. Resize and compress listing photos before upload, keep report evidence private, and watch storage usage.
- **Notifications:** Launch in-app notices and best-effort web push for new requests, Seller or Provider confirmations, cancellations, and new messages. A push sender and subscription storage must fit the free-service limits. Marketplace alerts must not depend on paid SMS or an email provider, and in-app deadlines remain visible when push is unavailable.
- **Operator:** The founder initially handles support, reports, and moderation through a protected admin view.

Monitor free-tier usage and keep recoverable copies of essential data. Free services have quotas and may pause projects with low activity. If those limits become a problem, revisit the operating plan before moving to paid infrastructure.

Recheck provider terms before deployment. Planning references: [Cloudflare Pages limits](https://developers.cloudflare.com/pages/platform/limits/), [Supabase pricing](https://supabase.com/pricing), [Supabase Google sign-in](https://supabase.com/docs/guides/auth/social-login/auth-google), [Supabase database webhooks](https://supabase.com/docs/guides/database/webhooks), [Supabase Edge Functions](https://supabase.com/docs/guides/functions), [Supabase free-project pausing](https://supabase.com/docs/guides/platform/free-project-pausing), and [WebKit's iOS web push guide](https://webkit.org/blog/13878/web-push-for-web-apps-on-ios-and-ipados/).
