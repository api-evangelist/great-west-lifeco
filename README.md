# Great-West Lifeco (great-west-lifeco)

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

Great-West Lifeco Inc. is a Winnipeg-headquartered international financial services holding company and a member of the Power Corporation group, and one of the largest life insurers in North America. It operates through Canada Life in Canada, the United Kingdom, the Isle of Man and Germany, through Irish Life in Ireland, and through Empower in the United States, spanning individual and group life, health and dental, disability and critical illness insurance, annuities and payout products, segregated funds and wealth management, employer-sponsored retirement recordkeeping, and life reinsurance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/great-west-lifeco/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/great-west-lifeco/refs/heads/main/apis.yml)

## API posture

Great-West Lifeco's home market is Canada, where OSFI supervises federally regulated insurers prudentially and the provinces (FSRA in Ontario, AMF in Quebec) regulate market conduct. There is no open-insurance mandate, and Consumer-Driven Banking — Canada's open-banking framework — excludes insurance entirely. Nothing forces a public API, and none exists.

The holding company publishes no developer surface, and neither does Canada Life, the Canadian operating brand. Probes of `developer.`, `developers.`, `docs.` and `api.` subdomains and of the `/developers`, `/api`, `/developer`, `/partners` and `/integrations` paths on both greatwestlifeco.com and canadalife.com returned no portal. The full public English sitemaps of both sites contain no API, developer, integration or ACORD page.

The one real developer surface in the group belongs to **Empower**, the U.S. retirement recordkeeping subsidiary. [developer.empower.com](https://developer.empower.com/) returns HTTP 200 and is a genuine developer portal with a publicly readable API catalog, getting-started guides, a documented authentication model, release notes and a status page. It is not self-serve: reference documentation sits behind login, and API keys and OAuth client credentials are issued only after an access request is reviewed and approved, then delivered by secure email. No OpenAPI, Swagger, AsyncAPI or public Postman artifact is published, and there is no ACORD, AL3 or IVANS reference anywhere on the group's public properties.

## Tags

- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Retirement
- Wealth Management
- Reinsurance
- Annuities
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

### Empower Balance API

Listed in the public API catalog of the Empower developer portal, operated by Great-West Lifeco's U.S. retirement subsidiary Empower. Marked "production" and categorized "financial", it returns participant-level balance data for employer-sponsored retirement plans, including total balances, investments, loans and vesting balances, in JSON. Reference documentation is gated behind login and access is granted only through the portal's request flow.

- **Human URL:** [https://developer.empower.com/api-catalog/balance-api](https://developer.empower.com/api-catalog/balance-api)

#### Properties

- [Documentation](https://developer.empower.com/api-catalog/balance-api)
- [Documentation](https://developer.empower.com/docs/get-started)

### Empower OAuth 2.0 API

The authorization API for Empower's API suite, listed as "production" in the public catalog. Public release notes document `/auth` and `/token` endpoints, an optional `x-api-key` header, and an `invalid_grant` 400 response when a requested OAuth scope is not configured on the client profile. Empower documents OAuth 2.0 and OpenID Connect with the `client_credentials` grant, moving to asymmetric `private_key_jwt` client authentication in support of Financial-grade API (FAPI) security.

- **Human URL:** [https://developer.empower.com/api-catalog/oauth2-api](https://developer.empower.com/api-catalog/oauth2-api)

#### Properties

- [Documentation](https://developer.empower.com/api-catalog/oauth2-api)
- [Authentication](https://developer.empower.com/docs/additional-security-protocols-publicprivate-key-infrastructure-pki)

## Links

- [Website](https://www.greatwestlifeco.com/)
- [About](https://www.greatwestlifeco.com/who-we-are/about-us.html)
- [News](https://www.greatwestlifeco.com/news-and-events/news.html)
- [Empower Retirement Developer Portal](https://developer.empower.com/)
- [Getting Started](https://developer.empower.com/docs/get-started)
- [Support](https://developer.empower.com/support)
- [Status and Maintenance](https://developer.empower.com/docs/status-and-maintenance)
- [Developer Terms of Use](https://developer.empower.com/DevTerms)

## Review

See [review.yml](review.yml) for the full API Evangelist review, including every probed URL and its HTTP status, the ACORD posture, the authentication model, and the reasoning behind the honest "partner-gated, no public specifications" finding.
