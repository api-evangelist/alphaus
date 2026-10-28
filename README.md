# Alphaus

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

Alphaus is a Tokyo-based cloud FinOps company (No. 1 in Japan) whose platform helps enterprises, managed service providers, and cloud resellers manage and optimize multi-cloud spend across AWS, Azure, and GCP. Its products include Octo (cost visibility and optimization), Ripple and WavePro (reseller billing automation and invoicing), and Cover (cost anomaly detection and recommendation intelligence). Developers integrate through the Blue API — a unified protobuf/gRPC surface with a grpc-gateway JSON/REST proxy and generated OpenAPI — spanning 15 services and nearly 600 operations, complemented by the bluectl CLI and Go, Python, and TypeScript SDKs.

**Areas:** Company · FinOps · Cloud Cost Management · Cloud · Billing · Multi-Cloud · AWS · Microsoft Azure · GCP · gRPC · Cost Optimization · Reseller Billing

## Alphaus on APIs.io

Everything profiled for Alphaus is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/alphaus/](https://apis.io/providers/alphaus/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Alphaus Admin API](https://apis.io/apis/alphaus/alphaus-admin-api/) — Admin API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Billing API](https://apis.io/apis/alphaus/alphaus-billing-api/) — (BETA) Billing API. Base URL: https://api.alphaus.cloud/m/blue/billing
- [Alphaus Cost API](https://apis.io/apis/alphaus/alphaus-cost-api/) — Cost API. Base URL: https://api.alphaus.cloud/m/blue/cost
- [Alphaus Cover API](https://apis.io/apis/alphaus/alphaus-cover-api/) — (BETA) Cover API. Base URL: https://api.alphaus.cloud/m/blue/cover
- [Alphaus Flags API](https://apis.io/apis/alphaus/alphaus-flags-api/) — (ALPHA) Flag API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Flow API](https://apis.io/apis/alphaus/alphaus-flow-api/) — (ALPHA) Flow API. Base URL: https://api.alphaus.cloud/m/blue/flow
- [Alphaus GuaranteedCommitments API](https://apis.io/apis/alphaus/alphaus-guaranteedcommitments-api/) — (Alpha) GuaranteedCommitments API. Base URL: https://api.alphaus.cloud/m/blue/gc
- [Alphaus Iam API](https://apis.io/apis/alphaus/alphaus-iam-api/) — (BETA) IAM API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Luster API](https://apis.io/apis/alphaus/alphaus-luster-api/) — (ALPHA) Luster API. Base URL: https://api.alphaus.cloud/m/blue/luster
- [Alphaus Operations API](https://apis.io/apis/alphaus/alphaus-operations-api/) — (BETA) Long operations API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Organization API](https://apis.io/apis/alphaus/alphaus-organization-api/) — (BETA) Organization API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Preferences API](https://apis.io/apis/alphaus/alphaus-preferences-api/) — (BETA) Preferences API. Base URL: https://api.alphaus.cloud/m/blue
- [Alphaus Pricing API](https://apis.io/apis/alphaus/alphaus-pricing-api/) — (BETA) Pricing API. Base URL: https://api.alphaus.cloud/m/blue/pricing
- [Alphaus Prism API](https://apis.io/apis/alphaus/alphaus-prism-api/) — (Alpha) Prism API. Base URL: https://api.alphaus.cloud/m/blue/prism
- [Alphaus Vortex API](https://apis.io/apis/alphaus/alphaus-vortex-api/) — (Alpha) Vortex API. Base URL: https://api.alphaus.cloud/m/blue/vortex

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [alphaus-blue](https://apis.io/servers/alphaus/alphaus-blue/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Alphaus Agentic Access](https://apis.io/agentic-access/alphaus/alphaus-agentic-access/)

#### Collections (15)

Postman and Open Collection request collections.

- [Blue API reference Admin API](https://apis.io/collections/alphaus/open-alphaus-admin-api/)
- [Blue API reference Admin Billing API](https://apis.io/collections/alphaus/open-alphaus-billing-api/)
- [Blue API reference Admin Cost API](https://apis.io/collections/alphaus/open-alphaus-cost-api/)
- [Blue API reference Admin Cover API](https://apis.io/collections/alphaus/open-alphaus-cover-api/)
- [Blue API reference Admin Flags API](https://apis.io/collections/alphaus/open-alphaus-flags-api/)
- [Blue API reference Admin Flow API](https://apis.io/collections/alphaus/open-alphaus-flow-api/)
- [Blue API reference Admin GuaranteedCommitments API](https://apis.io/collections/alphaus/open-alphaus-guaranteedcommitments-api/)
- [Blue API reference Admin Iam API](https://apis.io/collections/alphaus/open-alphaus-iam-api/)
- [Blue API reference Admin Luster API](https://apis.io/collections/alphaus/open-alphaus-luster-api/)
- [Blue API reference Admin Operations API](https://apis.io/collections/alphaus/open-alphaus-operations-api/)
- [Blue API reference Admin Organization API](https://apis.io/collections/alphaus/open-alphaus-organization-api/)
- [Blue API reference Admin Preferences API](https://apis.io/collections/alphaus/open-alphaus-preferences-api/)
- [Blue API reference Admin Pricing API](https://apis.io/collections/alphaus/open-alphaus-pricing-api/)
- [Blue API reference Admin Prism API](https://apis.io/collections/alphaus/open-alphaus-prism-api/)
- [Blue API reference Admin Vortex API](https://apis.io/collections/alphaus/open-alphaus-vortex-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Alphaus Blueapi Overlay](https://apis.io/overlays/alphaus/alphaus-blueapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Alphaus Authentication](https://apis.io/security/alphaus/alphaus-authentication/)
- [Alphaus Domain Security](https://apis.io/security/alphaus/alphaus-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Alphaus Scopes](https://apis.io/scopes/alphaus/alphaus-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://alphaus.cloud)
- [Documentation](https://labs.alphaus.cloud/docs/)
- [Getting started](https://labs.alphaus.cloud/docs/blueapi/overview/)
- [API reference](https://labs.alphaus.cloud/blueapidocs/)
- [Support](https://help.alphaus.cloud/en/)
- [Blog](https://labs.alphaus.cloud/blog/)
- [Terms of service](https://www.alphaus.cloud/en/ripple-wave-terms-of-services)
- [Privacy policy](https://www.alphaus.cloud/en/privacy)
- [GitHub](https://github.com/alphauslabs)
- [Status](https://status.alphaus.cloud/)

## API Evangelist rating

**Kin Score 51.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 38.7 |
| Contract governance | 4.5 |
| Operational transparency | 18.4 |
| Developer ergonomics | 73.2 |
| Access clarity | 27.6 |

**Agent readiness 20.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | mostly |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/alphaus/](https://apis.io/providers/alphaus/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Alphaus: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/alphaus/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
