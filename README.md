# UMart

UMart is a **UHome Community Marketplace** for items, food and drinks, services, and errands. The pilot tests whether people can find offers, agree on a Transaction, complete it, and return to use the app again instead of relying only on group-chat posts.

## Pilot scope

The mobile-friendly site will let anyone with the link browse public Listings. Google sign-in will be required to post, save, message, request, rate, or report. A UMart Member account does not verify UHome residency.

The planned pilot includes all four categories, dated stock or capacity, one Order Request per Listing, private messaging, Seller or Provider confirmation, Buyer-confirmed completion, ratings, moderation, in-app notices, and best-effort web push. Members arrange payment and handoff directly. The four-week pilot targets at least 20 Buyer-confirmed Transactions, 10 distinct Buyers, and 5 repeat Buyers, excluding founder/test activity and self-transactions.

## Planned tech stack

| Area | Plan |
| --- | --- |
| Web app | Responsive website hosted on Cloudflare Pages |
| Data and accounts | Supabase database, Google sign-in, and private storage |
| Notifications | In-app notices and web push where the browser supports it |

The frontend framework, development commands, and deployment configuration have not been selected or implemented yet. Hosting on free service tiers is a pilot target, subject to provider limits.

## Current status and local development

**Planning stage.** This repository contains product requirements, a build spec, and 28 implementation tickets. It has no application code or local start command yet. [Ticket 02](docs/planning/umart-pilot/issues/02-guest-live-listing-discovery.md) establishes the first running web path and its test setup. Once that work lands, this section should list the exact prerequisites, environment variables, install command, and local start command.

For now, clone the repository and review the planning files in a Markdown editor:

- [Product requirements](docs/planning/umart-pilot/PRODUCT.md)
- [Build spec](docs/planning/umart-pilot/spec.md)
- [Ticket overview and dependency order](docs/planning/umart-pilot/overview.md)
- [Domain glossary](CONTEXT.md) and [decision records](docs/adr/)

## Planned work

The tickets cover guest discovery and sign-in; Marketplace Listings and availability; messaging, Order Requests, and Transactions; Food Batches, Service Slots, and Errand Trips; reputation, moderation, support, notifications, pilot reporting, and hosted launch. Each ticket records its acceptance criteria and blockers. Developers and agents should read [AGENTS.md](AGENTS.md), the [build spec](docs/planning/umart-pilot/spec.md), and the relevant ticket before starting.
