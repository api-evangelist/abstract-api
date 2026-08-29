# Abstract API — OpenAPI specifications

Public OpenAPI 3.0.3 definitions for Abstract's API endpoints, for listing in API
directories ([APIs.guru](https://apis.guru/), RapidAPI, Postman) and for client / SDK generation.

Each file describes the **public HTTP interface only** — no source code, credentials, or secrets.
Every definition validates as OpenAPI 3.0.3 and shares one reviewed structure: dual auth
(`api_key` query **or** `Authorization: Bearer`), GET + POST (form-encoded or JSON) on every
path, and a common `{ "error": { message, code, details } }` error envelope.

- **Email Reputation** is additionally verified against the live production API.
- The other specs are generated from the [official documentation](https://docs.abstractapi.com)
  and follow the same conventions. Per-endpoint field nullability and the exact 422/429/500
  error strings are assumed generously and **pending production confirmation**.

To submit or consume a spec, use its raw URL:
`https://raw.githubusercontent.com/abstractapi/openapi-specs/main/<file>`

| API | Spec | Server | Paths |
|-----|------|--------|:-----:|
| Avatars | [`avatars.openapi.yaml`](./avatars.openapi.yaml) | `avatars.abstractapi.com/v1` | 1 |
| Company Enrichment | [`company-enrichment.openapi.yaml`](./company-enrichment.openapi.yaml) | `companyenrichment.abstractapi.com/v2` | 1 |
| Email Reputation | [`email-reputation.openapi.yaml`](./email-reputation.openapi.yaml) | `emailreputation.abstractapi.com/v1` | 1 |
| Exchange Rates | [`exchange-rates.openapi.yaml`](./exchange-rates.openapi.yaml) | `exchange-rates.abstractapi.com/v1` | 3 |
| IBAN Validation | [`iban-validation.openapi.yaml`](./iban-validation.openapi.yaml) | `ibanvalidation.abstractapi.com/v1` | 1 |
| IP Intelligence | [`ip-intelligence.openapi.yaml`](./ip-intelligence.openapi.yaml) | `ip-intelligence.abstractapi.com/v1` | 1 |
| Image Processing | [`images.openapi.yaml`](./images.openapi.yaml) | `images.abstractapi.com/v1` | 2 |
| Phone Intelligence | [`phone-intelligence.openapi.yaml`](./phone-intelligence.openapi.yaml) | `phoneintelligence.abstractapi.com/v1` | 1 |
| Public Holidays | [`holidays.openapi.yaml`](./holidays.openapi.yaml) | `holidays.abstractapi.com/v1` | 1 |
| Timezone | [`timezones.openapi.yaml`](./timezones.openapi.yaml) | `timezone.abstractapi.com/v1` | 2 |
| VAT Validation | [`vat-validation.openapi.yaml`](./vat-validation.openapi.yaml) | `vat.abstractapi.com/v1` | 3 |
| Web Scraping | [`scrape.openapi.yaml`](./scrape.openapi.yaml) | `scrape.abstractapi.com/v1` | 1 |
| Website Screenshot | [`screenshot.openapi.yaml`](./screenshot.openapi.yaml) | `screenshot.abstractapi.com/v1` | 1 |
