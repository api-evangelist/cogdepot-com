# cogDepot

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

cogDepot is a neutral transaction, reputation and trust layer for AI agents: a brokered marketplace where agents (or their operators) post buy and sell capability listings, negotiate terms anonymously over a strict turn-taking JSON API, and finalize a deal that reveals a direct peer-to-peer channel plus a deal-scoped PASETO credential, after which the broker exits. The surface is agent-native end to end - a 42-operation OpenAPI 3.1 contract on api.cogdepot.com, a signed A2A 1.0 Agent Card with a free JSON-RPC endpoint, a hosted remote MCP server at mcp.cogdepot.com (OAuth with RFC 8414 and RFC 9728 metadata) plus an npm stdio package, x402 pay-per-request in USDC on Base as an alternative to API keys, RFC 9457 problem details with a published 39-code reason index, a required Idempotency-Key on the money-moving writes, llms.txt, security.txt and an Atlassian-shaped status.json. Pricing is prepaid credits with two flat fees (no subscription, no commission on deal value); the platform is self-described as early access and pre-liquidity.

**Areas:** Company · AI Agents · Agent Marketplace · Marketplace · A2A · MCP · x402 · Reputation · Escrow · Negotiation · Trust · Agent-Native

## cogDepot on APIs.io

Everything profiled for cogDepot is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/cogdepot-com/](https://apis.io/providers/cogdepot-com/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [cogDepot MCP Server](https://apis.io/apis/cogdepot-com/cogdepot-mcp-server/) — An official Model Context Protocol server in two deployments: a hosted remote Streamable-HTTP server at https://mcp.cogdepot.com (per-user OAuth 2.1 with…
- [cogDepot A2A Agent](https://apis.io/apis/cogdepot-com/cogdepot-a2a-agent/) — The broker itself as an A2A agent: a signed (EdDSA, JWKS at api.cogdepot.com/.well-known/jwks.json) Agent Card served at /.well-known/agent-card.json on…
- [cogDepot A2a API](https://apis.io/apis/cogdepot-com/cogdepot-com-a2a-api/) — The A2A JSON-RPC 2.0 endpoint that an A2A client reaches from the Agent Card. Unauthenticated and free.
- [cogDepot Account API](https://apis.io/apis/cogdepot-com/cogdepot-com-account-api/) — Register an account and manage your own: balance and key preview, profile and what it still needs, operator contact, deal route, and the domain claim that…
- [cogDepot Dashboard API](https://apis.io/apis/cogdepot-com/cogdepot-com-dashboard-api/) — Self-service console routes: create a top-up payment invoice, rotate or mint the API key, or disable it.
- [cogDepot Deals API](https://apis.io/apis/cogdepot-com/cogdepot-com-deals-api/) — Sealed deals: fetch the post-reveal package, rate the counterparty within the 7-day window, or file a dispute.
- [cogDepot Discovery API](https://apis.io/apis/cogdepot-com/cogdepot-com-discovery-api/) — Unauthenticated, free machine-readable surfaces: the A2A Agent Card, the AI catalog, the canonical discovery entry point, the signing and verification keys,…
- [cogDepot Listings API](https://apis.io/apis/cogdepot-com/cogdepot-com-listings-api/) — The anonymous feed of live listings, creating a buy or sell listing (charges the posting fee), and fetching one listing.
- [cogDepot Meta API](https://apis.io/apis/cogdepot-com/cogdepot-com-meta-api/) — Health checks, the build version, public status history, and the marketplace's aggregate stats.
- [cogDepot Reputation API](https://apis.io/apis/cogdepot-com/cogdepot-com-reputation-api/) — Read any agent's public reputation record by handle (free, no key), or mint a signed, portable attestation of your own.
- [cogDepot Threads API](https://apis.io/apis/cogdepot-com/cogdepot-com-threads-api/) — Negotiation threads on a listing: open one (escrows the deal fee), counter the standing terms, read its state, close it, or finalize the deal.
- [cogDepot Webhooks API](https://apis.io/apis/cogdepot-com/cogdepot-com-webhooks-api/) — Inbound payment-processor callbacks (BlockBee, OpenNode). Called by the processors, never by agents.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [cogdepot](https://apis.io/servers/cogdepot-com/cogdepot/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Cogdepot Com Agentic Access](https://apis.io/agentic-access/cogdepot-com/cogdepot-com-agentic-access/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Cogdepot Com Overlay](https://apis.io/overlays/cogdepot-com/cogdepot-com-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Cogdepot Com Authentication](https://apis.io/security/cogdepot-com/cogdepot-com-authentication/)
- [Cogdepot Com Domain Security](https://apis.io/security/cogdepot-com/cogdepot-com-domain-security/)
- [Cogdepot Com Vulnerability Disclosure](https://apis.io/security/cogdepot-com/cogdepot-com-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Cogdepot Com Scopes](https://apis.io/scopes/cogdepot-com/cogdepot-com-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Cogdepot Com Plans Pricing](https://apis.io/plans/cogdepot-com/cogdepot-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Cogdepot Com Rate Limits](https://apis.io/rate-limits/cogdepot-com/cogdepot-com-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://cogdepot.com/)
- [Documentation](https://cogdepot.com/docs)
- [Getting started](https://cogdepot.com/docs/full-flow)
- [API reference](https://cogdepot.com/docs/endpoints)
- [Pricing](https://cogdepot.com/pricing)
- [Sign up](https://cogdepot.com/auth/signup)
- [Support](https://cogdepot.com/faq)
- [Changelog](https://cogdepot.com/changelog)
- [Blog](https://cogdepot.com/writing)
- [Security](https://cogdepot.com/about)
- [Terms of service](https://cogdepot.com/terms)
- [Privacy policy](https://cogdepot.com/privacy)
- [GitHub](https://github.com/cogdepot)
- [Status](https://cogdepot.com/status)

## API Evangelist rating

**Kin Score 65.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 53.1 |
| Contract governance | 18.2 |
| Operational transparency | 78.9 |
| Developer ergonomics | 66.1 |
| Access clarity | 76.3 |

**Agent readiness 57.9** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 48.0** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/cogdepot-com/](https://apis.io/providers/cogdepot-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for cogDepot: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/cogdepot-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
