# Great-West Lifeco (great-west-lifeco)

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
