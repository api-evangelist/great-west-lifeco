# Great-West Lifeco

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

Great-West Lifeco Inc. is a Winnipeg-headquartered international financial services holding company and a member of the Power Corporation group, and one of the largest life insurers in North America. It operates through Canada Life in Canada, the United Kingdom, the Isle of Man and Germany, through Irish Life in Ireland, and through Empower in the United States, spanning individual and group life, health and dental, disability and critical illness insurance, annuities and payout products, segregated funds and wealth management, employer-sponsored retirement recordkeeping, and life reinsurance. Its home market is Canada, where it is federally supervised by OSFI for prudential matters while market conduct is regulated province by province, and where no open-insurance mandate exists (Consumer-Driven Banking excludes insurance outright). Its API posture reflects that absence of a forcing function: the Great-West Lifeco corporate site and the Canadian consumer site canadalife.com publish no developer portal and no API documentation, and probes of developer/docs subdomains and /developers, /api, /developer, /partners and /integrations paths return no such surface. Two production API surfaces nevertheless exist inside the group, both partner-gated and unrelated to each other. Canada Life runs an Apigee gateway at api.canadalife.com that serves a real OpenID Connect discovery document anonymously - issuer, JWKS, token, revocation and userinfo endpoints, with the authorization endpoint deliberately published as "authorize-NOT-SUPPORTED" and an empty scopes_supported array - and whose error envelopes point to https://apimarketplace.canadalife.com, a digitalML-hosted API marketplace that does not resolve publicly. The U.S. retirement subsidiary Empower runs a genuine developer portal that lists two production APIs publicly while naming eight API products plus three coming soon on its marketing site, places every piece of reference documentation behind login, documents an x-api-key header with OAuth 2.0 client_credentials and private_key_jwt in support of FAPI, publishes release notes, a maintenance window and a mock-data sandbox, and issues credentials only after a reviewed access request. There is no downloadable OpenAPI anywhere, no public Postman collection, no SDK, no MCP server, no webhook or event catalog, and no ACORD, AL3 or IVANS reference on any public property in the group.

**Areas:** Insurance · Canada · Life Insurance · Health Insurance · Employee Benefits · Retirement · Wealth Management · Reinsurance · Annuities

## Great-West Lifeco on APIs.io

Everything profiled for Great-West Lifeco is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/great-west-lifeco/](https://apis.io/providers/great-west-lifeco/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Empower Balance API](https://apis.io/apis/great-west-lifeco/empower-balance-api/) — Listed in the public API catalog of the Empower developer portal, operated by Great-West Lifeco's U.S. retirement subsidiary Empower. Marked "production"…
- [Empower OAuth 2.0 API](https://apis.io/apis/great-west-lifeco/empower-oauth-2-0-api/) — The authorization API for Empower's API suite, listed as "production" in the public Empower developer portal catalog. It generates bearer access tokens used…
- [Canada Life API Gateway (OAuth 2.0 / OpenID Connect)](https://apis.io/apis/great-west-lifeco/canada-life-api-gateway/) — The production API gateway of Canada Life, Great-West Lifeco's Canadian operating brand, at api.canadalife.com. It publishes no documentation, but it does…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Great West Lifeco Authentication](https://apis.io/security/great-west-lifeco/great-west-lifeco-authentication/)
- [Great West Lifeco Domain Security](https://apis.io/security/great-west-lifeco/great-west-lifeco-domain-security/)
- [Great West Lifeco Trust Center](https://apis.io/security/great-west-lifeco/great-west-lifeco-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Great West Lifeco Scopes](https://apis.io/scopes/great-west-lifeco/great-west-lifeco-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.greatwestlifeco.com/)
- [Documentation](https://developer.empower.com/docs/get-started)
- [Getting started](https://developer.empower.com/docs/get-started)
- [API reference](https://developer.empower.com/api-catalog)
- [Sign up](https://developer.empower.com/hybridauth-connect/authenticate/cognito)
- [Support](https://developer.empower.com/support)
- [Compliance](https://www.empower.com/financial-professionals/about-empower/cybersecurity)
- [Terms of service](https://developer.empower.com/DevTerms)
- [Privacy policy](https://www.greatwestlifeco.com/privacy-policy.html)
- [Status](https://developer.empower.com/docs/status-and-maintenance)

## API Evangelist rating

**Kin Score 40.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 72.3 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 36.8 |
| Developer ergonomics | 61.9 |
| Access clarity | 50.0 |

**Agent readiness 9.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 41.2** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/great-west-lifeco/](https://apis.io/providers/great-west-lifeco/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Great-West Lifeco: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/great-west-lifeco/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
