# UMart — Product Requirements

## 1. Product Summary

**UMart** is a private community marketplace for people who live in the same dormitory, residential building, or university community.

It gives community members one place to discover and interact with people offering:

- Used and pre-loved items
- Food and drinks
- Services
- Errands and pasabuy
- Other community-based products or offerings

UMart is initially being tested within **UHome / University Home**. UHome will serve as the first community, but the product is designed so the same platform can eventually support other dorms, residences, condos, and university communities.

The initial release is a mobile-friendly website shared through the UHome group chat. Residents can optionally add it to their phone's home screen. UMart is free for residents to use; initial hosting aims to stay within free-service limits.

### Core value proposition

For consumers:
> Find useful products, food, services, and errands from people within your community.

For sellers/providers:
> Offer products or services to your community without repeatedly posting in a group or exposing personal social-media accounts.

For the community:
> Have one organized place to discover what people nearby are offering.

---

## 2. Product Vision

UMart should feel like a **small, community-specific version of a marketplace/social platform**, rather than a full-scale food-delivery company.

The product combines:

**Community discovery + Marketplace + Messaging + Order Requests**

The central product idea is:

> **People in the same community can discover what others are offering, communicate privately, and organize transactions without needing to exchange personal social accounts.**

UMart is not intended to become a general-purpose social network, payment processor, or delivery company.

---

## 3. Initial Community: UHome

### UHome MVP

The first version of UMart will be tested with **UHome tenants**.

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

UMart should use a **public username / private resident information** model rather than full anonymity.

### Public profile

Example:

```text
@Mika
UHome member
📍 30th Floor
```

Users do **not** need to expose their:

- Facebook account
- Instagram account
- Personal social profiles
- Phone number
- Other personal contact information

### Room information

A user's exact room number may be collected as part of their community profile, but it should **not be publicly displayed by default**.

Only the user's floor should normally appear publicly.

For example:

```text
Public:
@Mika
UHome member
30th Floor

Private:
Room 3021
```

When a transaction requires coordination, the buyer and seller can voluntarily disclose their exact room number or another meeting point through their conversation.

Possible pickup locations include:

- UHome lobby
- Common area
- A mutually agreed floor/location
- A user's room, only if both parties voluntarily agree

### Important privacy principle

UMart should make **exact residential location private by default**.

---

## 5. Community Access & Verification

UMart is intended to be community-based, but the MVP does **not** depend on UHome administration or an official partnership with UHome.

This is intentional because requiring administrators to manually verify users or perform ongoing work would create an unnecessary dependency during early testing.

### MVP approach

The initial launch link will be shared in the UHome community group chat. A forwarded link could reach someone outside the group, so distribution through the chat does not itself establish residency. Describe the launch as **launched for the UHome community** without implying that every member is a verified tenant. Stronger access controls can be added if needed later.

Initial login uses **Sign in with Google**. The Google account identifies the user privately; their UMart username is displayed publicly. Their Google profile and email address are not displayed to other members.

### Verification status

UMart should **not claim “Verified UHome Resident”** unless there is an actual verification process behind that label.

A stronger verification system can be introduced later if UMart expands and gains formal partnerships or a reliable way to verify residency.

---

## 6. Core Marketplace Categories

### 6.1 Marketplace

In the navigation, **Marketplace** is the category for physical items. UMart as a whole includes Marketplace, Food & Drinks, Services, and Errands / Pasabuy. Residents can list new or used items.

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
- Floor

---

### 6.2 Food & Drinks

Residents can sell food and beverages directly to other community members.

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
- Stock/quantity
- Availability
- Pre-order settings
- Pickup/delivery method
- Seller
- Floor

---

### 6.3 Services

Residents can offer services to other community members.

Examples:

- Tutoring
- Printing
- Laundry
- Haircuts
- Repairs
- Graphic design
- Photography
- Tech assistance
- Other useful resident-to-resident services

A service listing should support:

- Service description
- Price or rate
- Availability
- Provider
- Floor
- Request/contact flow

---

### 6.4 Errands / Pasabuy

Residents can offer to perform errands for other residents.

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

The goal is for users to quickly understand what is actually available instead of seeing outdated community posts.

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

When enabled, a pre-order has an opening time, cutoff, fulfillment date or window, and stock or capacity. Buyers can submit requests while the order window is open. The seller must still confirm each request; submitting one does not reserve stock.

---

## 9. “Available Now” Discovery

The home experience should prioritize offerings that are currently available or becoming available soon.

**Available Now** appears only while the offering is within its availability window, has stock or capacity where applicable, and is not paused. A future batch may instead show **Pre-order Open** while its request window is open.

Example:

```text
AVAILABLE NOW

🍵 Matcha by @Mika
₱120
30th Floor
Available until 10 PM

🍪 Cookies by @Anne
₱80
28th Floor
8 boxes remaining

🏃 Pasabuy — SM
30th Floor
Leaving at 6:30 PM
```

This is a key distinction from a conventional community feed where posts can quickly become buried or outdated.

---

## 10. Seller / Provider Profiles

Each seller/provider should have a persistent UMart profile rather than relying on repeated social-media posts.

Example:

```text
@Mika
UHome member
📍 30th Floor

⭐ 4.9
24 completed transactions

ABOUT
Matcha and drinks made to order.

LISTINGS
Classic Matcha — ₱120
Strawberry Matcha — ₱140
Dirty Matcha — ₱150
```

Each public profile can show separate **seller/provider** and **buyer** rating summaries, including the number of ratings behind each average. A member can have both kinds of reputation.

The account owner's profile also shows their **private buying and selling history**: the item or service, other party, agreed terms, and current status. Only the transaction participants and a moderator handling a report or support issue may see these details. Other members can see public listings and ratings, but not someone's purchase history or conversations.

A resident can simultaneously be a:

- Consumer
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
Floor: 30
Stock: 10
Availability: 6 PM–10 PM
Pre-order: Available

[Request Order]
```

This structure makes information searchable, filterable, and easier to act on.

---

## 12. Messaging

UMart should include built-in messaging so users can communicate without exchanging personal social-media accounts.

Messaging should support conversations connected to a listing or order request.

Example:

```text
Buyer:
Is this still available?

Seller:
Yes. I can prepare it around 7 PM.
```

Messaging is important because UMart does **not** attempt to fully automate community transactions.

The users can discuss and agree on the practical details themselves.

---

## 13. Order Request Model

UMart should **not treat a button press as a guaranteed purchase or booking**.

When a consumer selects **Order / Request**, UMart creates an **Order Request** and notifies the seller. It records the listing, requested quantity or scope, proposed schedule and arrangement, and both participants.

### Core flow

```text
Customer submits Order Request
            ↓
Seller receives notification
            ↓
Seller and customer communicate; seller may mark it Discussing
            ↓
Details are agreed upon
            ↓
Seller confirms agreed terms
            ↓
Order becomes Confirmed
            ↓
Transaction is fulfilled directly between the parties
            ↓
Seller marks the transaction Completed; both parties may review
```

### Why this model is used

The seller needs the ability to confirm that:

- The product is actually available
- The requested quantity is possible
- The stated price is still correct
- The seller can fulfill the request
- The pickup/delivery arrangement works
- The customer and seller have agreed on the final details

This also reduces the impact of fake bookings or accidental requests.

### Order statuses

- **Pending Request** — Buyer submitted a request; no sale, booking, or stock reservation is guaranteed.
- **Discussing** — Seller marked the request as needing clarification. The terms are not confirmed yet.
- **Confirmed** — Seller accepted and recorded the agreed quantity or scope, final price or fee, fulfillment time, and pickup or delivery arrangement. Confirmation cannot exceed available stock or capacity.
- **Completed** — Seller marked a confirmed transaction fulfilled. Only the seller can make this status change.
- **Declined** — Seller rejected a request before confirming it.
- **Cancelled** — A pending, discussing, or confirmed request will no longer proceed. Either party can cancel, with a reason recorded and the other party notified. Completed transactions instead use the report flow if disputed.

Both participants see the current status and agreed details in their private order histories and linked conversation. A seller can move a request to **Discussing** without promising to fulfill it. If a buyer disputes a seller's **Completed** status, they can leave an honest review and/or report the transaction. The moderator can investigate and correct a false completion and its associated reviews.

For a physical item or food order, a seller may also notify the buyer that a **Confirmed** order is ready for pickup. This is a fulfillment update; it does not itself mark the order Completed.

---

## 14. Inventory Behavior

A request should **not automatically become a confirmed sale**.

Likewise, inventory should not be permanently deducted merely because someone tapped Order.

For limited-stock items, stock should become committed only when the seller confirms the request. Confirming must check and commit available stock in one operation so competing requests cannot claim the same last item. Cancelling a confirmed request returns its committed stock; completing it does not. The same rule applies to limited service or errand slots.

This is particularly important for food and drink sellers who prepare a limited quantity each day.

---

## 15. Payments

UMart will **not process payments during the MVP**.

The actual payment is handled directly between the seller/provider and the consumer.

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

The consumer collects the item/order from an agreed location.

### Seller delivery

The seller/provider delivers personally when they choose to.

### Community errands

Another UMart member can fulfill the request through an errand/pasabuy listing.

---

## 17. Ratings & Reputation

After the **seller marks a confirmed transaction Completed**, each party can optionally leave one rating and review for the other party:

- **Buyer rates seller/provider** for the offering and their experience. The review appears on the seller/provider's public profile.
- **Seller/provider rates buyer** for their experience, such as communication and following the agreed arrangement. The review appears on the buyer's public profile.

Reviews must be linked to a completed transaction and show whether the author was the buyer or seller. Public reviews should not reveal room numbers, contact information, private order details, or conversation messages. A buyer can report a false completion; the moderator can remove ratings associated with a fabricated or abusive transaction.

Example:

```text
⭐ 5.0
Fast response and good matcha.
```

Profiles can show:

- Completed transactions by role
- Separate buyer and seller rating averages and rating counts
- Buyer and seller review history

Buyer and seller ratings are counted separately and are only associated with **completed transactions**, rather than allowing arbitrary reviews from people who never transacted.

---

## 18. Safety & Moderation

The MVP should provide basic community safety controls.

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

Safety features should be simple enough for an MVP but should exist from the beginning because UMart facilitates interactions involving money, food, and physical meetups.

---

## 19. Notifications

UMart should notify users about meaningful marketplace, messaging, order, and support events.

Examples:

- New order request
- New message
- Order request accepted
- Order request declined
- Order confirmed
- Order marked for discussion
- Order ready
- Order cancelled
- Seller marked transaction completed
- New buyer or seller review
- Listing sold/completed
- Support ticket update
- Report status update, when appropriate

The MVP does not need an elaborate notification-preferences system.

---

## 20. Onboarding

UMart should include a short first-time onboarding flow so new users understand how the app works before using the marketplace.

The onboarding should be brief, visual, and focused on the concepts a user needs to understand immediately.

### Core onboarding topics

1. **What is UMart?**
   - A marketplace for people within the same community.

2. **What can you do?**
   - Buy and sell items
   - Order food and drinks
   - Offer services
   - Offer or request errands/pasabuy

3. **How does privacy work?**
   - Users have a UMart username
   - Only their floor is public by default
   - Their exact room number is private
   - Personal social-media accounts do not need to be shared

4. **How do order requests work?**
   - A customer submits a request
   - The seller receives a notification
   - The seller and customer communicate
   - The seller may discuss details before confirming whether the transaction will proceed
   - Payment and fulfillment happen directly between the parties

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
- How does seller confirmation work?
- How does pre-ordering work?
- How do availability schedules work?
- Does UMart process payments?
- How are payments handled?
- How do pickup and delivery work?
- Can other users see my room number?
- How do messaging and order conversations work?
- How do ratings and reviews work?
- What should I do if a seller or customer does not respond?
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

For payment-related concerns, UMart can document and review the reported issue, but the actual payment remains a direct transaction between the seller and consumer. UMart does not act as the payment intermediary.

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

---

## 23. Community / Social Layer

UMart can have a lightweight community-feed feeling similar to Facebook, but only within the context of community commerce.

The **Home feed** shows listings from all four UMart categories together: Food & Drinks, Marketplace, Services, and Errands / Pasabuy. It is a general view of community offerings, while each listing remains a structured item that can be searched, filtered, and requested.

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

General feed of offerings across all four categories, with clear **Available Now** and **Pre-order Open** labels. Show four visible category shortcuts: **Food & Drinks**, **Marketplace**, **Services**, and **Errands / Pasabuy**. Tapping one opens Explore with that category already selected. Category discovery should use visible controls rather than requiring a user to swipe through category pages.

### Explore

Search and category browsing. The selected category determines which filters and sorting choices appear:

| Category | Filters | Sorting |
| --- | --- | --- |
| Food & Drinks | Drinks, meals, snacks, desserts; available now or pre-order; price range | Newest or price |
| Marketplace | Furniture, electronics, appliances, clothes, and other items; condition; price range | Newest or price |
| Services | Service type; availability; price range | Newest or price |
| Errands / Pasabuy | No subcategory filters required initially | No category-specific sorting required initially |

Choosing a type such as **Furniture** filters which listings are shown; choosing **Price: Low to High** sorts their order. Search can work across all categories or within the one currently selected.

### Orders

Private buying and selling history, including pending, discussing, confirmed, completed, declined, and cancelled requests.

### Inbox

Buyer/seller conversations.

### Profile

User profile, public buyer and seller ratings, listings, availability, private buying and selling history for the account owner, and account/help access.

---

## 25. Initial User Types

### Consumer

Can:

- Browse
- Search
- View listings
- Message sellers/providers
- Submit order requests
- Request services/errands
- Complete transactions
- Review completed transactions
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
- Message customers
- Accept/decline requests
- Confirm transactions
- Mark transactions completed
- Optionally review buyers after marking confirmed transactions completed
- View their private selling history and seller rating

### Errand Provider

Can:

- Create an errand/pasabuy listing
- Set destination
- Set schedule
- Set service fee
- Accept requests
- Communicate with requesters
- Complete requests

These are not separate account types. A single UMart member can perform all of these activities.

### Moderator / Admin

Can:

- Review reports
- Review support requests
- Remove listings/content
- Suspend or restrict accounts
- Moderate the community

---

## 26. MVP Scope

### Must Have

- UHome community
- UHome group-chat link distribution, without a claim of verified residency
- User accounts
- Public username/display identity
- Private room information
- Public floor information
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
- Optional seller-enabled pre-ordering for food and drinks
- Available-now discovery
- Listing details
- In-app messaging
- Order requests
- Seller notification for order requests
- Seller/customer conversation flow
- Seller confirmation flow
- Order status tracking
- Transaction completion
- Optional, transaction-linked ratings/reviews in both directions after seller-marked completion
- Separate public buyer and seller ratings, with private buying and selling history
- Report member/listing/transaction functionality
- Evidence attachments for reports
- Basic moderation tools
- FAQ/help center
- User support / issue reporting
- Basic onboarding
- Basic notifications
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

UMart is built around people who physically share the same community.

### 2. Privacy by default

Users should be able to transact without exposing personal social-media accounts or exact room information publicly.

### 3. Structured commerce

UMart should turn informal community posts into useful, searchable listings with price, stock, availability, and ordering information.

### 4. Human confirmation

UMart facilitates the transaction, but the seller and consumer remain responsible for agreeing on the final deal.

### 5. No unnecessary middleman

Payments and physical fulfillment remain between the parties during the MVP.

### 6. Community accountability

Users can report problematic behavior and provide evidence, while moderators review reports before taking action.

### 7. Small first

UHome is the first real-world test. Features should be built to solve UHome's actual problems before expanding into a broader platform.

---

## 28. The Core User Experience

The target experience is:

> Open UMart → see what is available around UHome → find a product/service/errand → view the seller/provider → submit a request → receive/respond to messages → agree on the details → seller confirms → complete the transaction.

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
UHome member
30th Floor

10 available
6 PM–10 PM
Pre-order available

[Request Order]
```

The goal is not to remove the human conversation. The goal is to make the conversation happen **around an organized listing and transaction**.

---

## 30. Product Success Question

The most important validation question for UMart is not whether the software can be built.

It is:

> **Why would a UHome resident use UMart instead of posting in the existing community group?**

UMart must prove that the combination of:

- Better discovery
- Structured listings
- Availability and pre-orders
- In-app communication
- Seller profiles
- Community context
- Reduced need to expose personal social accounts
- A clear request/confirmation flow

creates enough value for residents to change their behavior.

The first UHome test should therefore focus on **real usage and completed community transactions**, not feature count.

---

## 31. Initial Build & Operating Cost

UMart should be free for residents to use at launch. Aim to keep initial hosting at **₱0** while remaining within free-service limits; this is an operating target, not a promise that unlimited usage is free.

- **Website:** A mobile-friendly site hosted on Cloudflare Pages using its provided `pages.dev` address, so an initial custom domain is unnecessary.
- **Application data and accounts:** Supabase Free for Google sign-in, profiles, listings, messages, requests, reviews, and reports. Enforce authorization on data so only the appropriate users and moderator can access private records.
- **Images and evidence:** Start with free storage. Resize and compress listing photos before upload, keep report evidence private, and watch storage usage.
- **Notifications:** Start with notifications inside the site. Marketplace alerts must not depend on paid SMS or an email provider.
- **Operator:** The founder initially handles support, reports, and moderation through a protected admin view.

Monitor free-tier usage and keep recoverable copies of essential data. Free services have quotas and may pause projects with low activity. If those limits become a problem, revisit the operating plan before moving to paid infrastructure.

Recheck provider terms before deployment. Planning references (checked October 2026): [Cloudflare Pages limits](https://developers.cloudflare.com/pages/platform/limits/), [Supabase pricing](https://supabase.com/pricing), [Supabase Google sign-in](https://supabase.com/docs/guides/auth/social-login/auth-google), and [Supabase free-project pausing](https://supabase.com/docs/guides/platform/free-project-pausing).
