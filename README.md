# Phasio

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Phasio is an operating platform for manufacturing service providers that unifies intelligent quoting, production operations, connected back-office/ERP integration, part intelligence, and white-labeled customer storefronts. It serves contract manufacturers across additive manufacturing, CNC machining, and injection molding, generating CAD-based quotes in seconds and managing shop-floor routing and scheduling. The Phasio Manufacturer REST API (v1, base /api/manufacturer/v1) is published as an OpenAPI 3.2 contract of 130 operations across 32 resource groups covering orders, carts, customers and customer organisations, addresses, part revisions and specifications, requisitions and work orders, production steps and routing templates, documents, payments, shipments and shipping rates, and webhooks, authenticated with a Bearer API key created under Settings > API Keys.

**Areas:** Company · Manufacturing · 3D Printing · CNC Machining · Quoting · Production Operations · Manufacturing Execution

## Phasio on APIs.io

Everything profiled for Phasio is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/phasio/](https://apis.io/providers/phasio/)** — or go straight to one of the APIs or properties below.

### APIs (32)

- [Phasio Addresses API](https://apis.io/apis/phasio/phasio-addresses-api/) — API for managing addresses for customers and organizations
- [Phasio Cart Resource API](https://apis.io/apis/phasio/phasio-cart-resource-api/) — Read storefront carts, a single cart, and a cart's pre-order (quote and purchasability).
- [Phasio Manufacturer Activity Controller API](https://apis.io/apis/phasio/phasio-manufacturer-activity-controller-api/) — Endpoints for managing manufacturer activities and conversations
- [Phasio Manufacturer Analytics Controller API](https://apis.io/apis/phasio/phasio-manufacturer-analytics-controller-api/) — Programmatic analytics endpoints for retrieving manufacturer dashboard metrics, funnel performance, revenue, production, customer and material insights.
- [Phasio Manufacturer Assembly Controller API](https://apis.io/apis/phasio/phasio-manufacturer-assembly-controller-api/) — Endpoints for managing assemblies
- [Phasio Manufacturer CAMSPEC Controller API](https://apis.io/apis/phasio/phasio-manufacturer-camspec-controller-api/) — Endpoints for exporting CAMSPEC files and managing manifest mappings
- [Phasio Manufacturer Cart Item Controller API](https://apis.io/apis/phasio/phasio-manufacturer-cart-item-controller-api/) — API for managing cart items
- [Phasio Manufacturer Catalog Controller API](https://apis.io/apis/phasio/phasio-manufacturer-catalog-controller-api/) — Endpoints for managing manufacturer catalog items
- [Phasio Manufacturer Color Controller API](https://apis.io/apis/phasio/phasio-manufacturer-color-controller-api/) — Endpoints for retrieving color options for manufactured parts
- [Phasio Manufacturer Customer Controller API](https://apis.io/apis/phasio/phasio-manufacturer-customer-controller-api/) — API for managing customer records and operations
- [Phasio Manufacturer Customer Organisation Controller API](https://apis.io/apis/phasio/phasio-manufacturer-customer-organisation-controller-api/) — API for managing customer organizations
- [Phasio Manufacturer Document Controller API](https://apis.io/apis/phasio/phasio-manufacturer-document-controller-api/) — API for generating and downloading various document types
- [Phasio Manufacturer Document Template Controller API](https://apis.io/apis/phasio/phasio-manufacturer-document-template-controller-api/) — Endpoints for managing document templates for invoices, orders, and consignment labels
- [Phasio Manufacturer Infill Controller API](https://apis.io/apis/phasio/phasio-manufacturer-infill-controller-api/) — Endpoints for managing 3D printing infill options and configurations
- [Phasio Manufacturer Kanban Column Controller API](https://apis.io/apis/phasio/phasio-manufacturer-kanban-column-controller-api/) — Endpoints for managing Kanban board columns for order processing workflow
- [Phasio Manufacturer Material Controller API](https://apis.io/apis/phasio/phasio-manufacturer-material-controller-api/) — Endpoints for managing manufacturing materials
- [Phasio Manufacturer Part Revision Controller API](https://apis.io/apis/phasio/phasio-manufacturer-part-revision-controller-api/) — Endpoints for managing part geometry revisions and 3D file analysis
- [Phasio Manufacturer Part Specification Controller API](https://apis.io/apis/phasio/phasio-manufacturer-part-specification-controller-api/) — Endpoints for managing part specifications and customer article references
- [Phasio Manufacturer Post Processing Controller API](https://apis.io/apis/phasio/phasio-manufacturer-post-processing-controller-api/) — Endpoints for managing post-processing options for manufactured parts
- [Phasio Manufacturer Precision Prices Controller API](https://apis.io/apis/phasio/phasio-manufacturer-precision-prices-controller-api/) — Endpoints for managing precision prices for manufacturing operations
- [Phasio Manufacturer Process Prices Controller API](https://apis.io/apis/phasio/phasio-manufacturer-process-prices-controller-api/) — Endpoints for managing manufacturing process pricing configurations
- [Phasio Manufacturer Production Step Controller API](https://apis.io/apis/phasio/phasio-manufacturer-production-step-controller-api/) — Endpoints for managing production steps in the manufacturing workflow
- [Phasio Manufacturer Requisition Controller API](https://apis.io/apis/phasio/phasio-manufacturer-requisition-controller-api/) — API for managing part requisitions and production batches
- [Phasio Manufacturer Routing Template Controller API](https://apis.io/apis/phasio/phasio-manufacturer-routing-template-controller-api/) — Manage routing templates on a part specification
- [Phasio Manufacturer Thread File Controller API](https://apis.io/apis/phasio/phasio-manufacturer-thread-file-controller-api/) — API for managing files attached to threads
- [Phasio Manufacturer Work Order Controller API](https://apis.io/apis/phasio/phasio-manufacturer-work-order-controller-api/) — Manage individual work orders, including downstream routing mutations
- [Phasio Webhooks API](https://apis.io/apis/phasio/phasio-webhooks-api/) — Endpoints for managing webhooks
- [Phasio Operator Addresses API](https://apis.io/apis/phasio/phasio-operator-addresses-api/) — API for managing manufacturer operator addresses
- [Phasio Orders API](https://apis.io/apis/phasio/phasio-orders-api/) — API for managing orders and their lifecycle
- [Phasio Payments API](https://apis.io/apis/phasio/phasio-payments-api/) — Manage payments for orders
- [Phasio Shipments API](https://apis.io/apis/phasio/phasio-shipments-api/) — Create, replace, and progress shipments on an order
- [Phasio Shipping Rates API](https://apis.io/apis/phasio/phasio-shipping-rates-api/) — API for retrieving shipping rates for parts

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Phasio Webhooks](https://apis.io/asyncapis/phasio/phasio-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [phasio](https://apis.io/servers/phasio/phasio/)

#### Collections (32)

Postman and Open Collection request collections.

- [Phasio Addresses API](https://apis.io/collections/phasio/open-phasio-addresses-api/)
- [Phasio Cart Resource API](https://apis.io/collections/phasio/open-phasio-cart-resource-api/)
- [Phasio Manufacturer Activity Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-activity-controller-api/)
- [Phasio Manufacturer Analytics Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-analytics-controller-api/)
- [Phasio Manufacturer Assembly Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-assembly-controller-api/)
- [Phasio Manufacturer CAMSPEC Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-camspec-controller-api/)
- [Phasio Manufacturer Cart Item Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-cart-item-controller-api/)
- [Phasio Manufacturer Catalog Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-catalog-controller-api/)
- [Phasio Manufacturer Color Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-color-controller-api/)
- [Phasio Manufacturer Customer Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-customer-controller-api/)
- [Phasio Manufacturer Customer Organisation Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-customer-organisation-controller-api/)
- [Phasio Manufacturer Document Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-document-controller-api/)
- [Phasio Manufacturer Document Template Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-document-template-controller-api/)
- [Phasio Manufacturer Infill Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-infill-controller-api/)
- [Phasio Manufacturer Kanban Column Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-kanban-column-controller-api/)
- [Phasio Manufacturer Material Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-material-controller-api/)
- [Phasio Manufacturer Part Revision Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-part-revision-controller-api/)
- [Phasio Manufacturer Part Specification Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-part-specification-controller-api/)
- [Phasio Manufacturer Post Processing Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-post-processing-controller-api/)
- [Phasio Manufacturer Precision Prices Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-precision-prices-controller-api/)
- [Phasio Manufacturer Process Prices Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-process-prices-controller-api/)
- [Phasio Manufacturer Production Step Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-production-step-controller-api/)
- [Phasio Manufacturer Requisition Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-requisition-controller-api/)
- [Phasio Manufacturer Routing Template Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-routing-template-controller-api/)
- [Phasio Manufacturer Thread File Controller API](https://apis.io/collections/phasio/open-phasio-manufacturer-thread-file-controller-api/)
- …and 7 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Phasio Manufacturer Overlay](https://apis.io/overlays/phasio/phasio-manufacturer-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Phasio Authentication](https://apis.io/security/phasio/phasio-authentication/)
- [Phasio Domain Security](https://apis.io/security/phasio/phasio-domain-security/)
- [Phasio Trust Center](https://apis.io/security/phasio/phasio-trust-center/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Phasio Plans Pricing](https://apis.io/plans/phasio/phasio-plans-pricing/)
- [Phasio Price Estimates](https://apis.io/plans/phasio/phasio-price-estimates/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://phas.io)
- [Documentation](https://docs.phas.io/developers)
- [Getting started](https://docs.phas.io/developers)
- [API reference](https://docs.phas.io/developers)
- [Pricing](https://phas.io/pricing)
- [Sign up](https://auth.phas.io/create)
- [Support](https://phas.io/contact)
- [Blog](https://phas.io/post)
- [Compliance](https://phas.io/security)
- [Terms of service](https://phas.io/terms-of-service)
- [Privacy policy](https://phas.io/privacy-policy)

## API Evangelist rating

**Kin Score 57.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 57.5 |
| Contract governance | 18.2 |
| Operational transparency | 7.9 |
| Developer ergonomics | 58.9 |
| Access clarity | 81.6 |

**Agent readiness 44.0** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly |

**Regulatory alignment 29.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/phasio/](https://apis.io/providers/phasio/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Phasio: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/phasio/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
