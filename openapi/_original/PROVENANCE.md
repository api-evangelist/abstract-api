# Provider-published OpenAPI — harvested verbatim

Source: <https://github.com/abstractapi/openapi-specs> (branch `main`), fetched 2026-08-29
via `https://raw.githubusercontent.com/abstractapi/openapi-specs/main/<file>` — HTTP 200 on
all 13 files.

**Ownership check (STEP 0c).** Every file declares `servers[]` on `*.abstractapi.com`,
`info.title` beginning "Abstract", and the repository lives in the `abstractapi` GitHub
organization already recorded as this provider's `GitHubOrganization` in `apis.yml`. The
upstream README (`UPSTREAM-README.md`) is written in Abstract's own voice and links
`docs.abstractapi.com`. The contract belongs to this company.

**Why this matters.** Until this pass the repo's `openapi/*.yml` were API Evangelist–authored
definitions written from the documentation (archived under `openapi/_ae-authored/`). Abstract
publishes its own definitions, and they are strictly richer: every path carries **both GET and
POST** (the AE-authored specs carried GET only), and two endpoints exist upstream that the
AE-authored set never had — `POST/GET /upload` on Image Processing and `/categories` on VAT
Validation.

**Divergences worth carrying forward into the next `refine-openapis` pass:**

| Product | AE-authored | Provider-published | Verdict |
|---|---|---|---|
| Company Enrichment | `companyenrichment.abstractapi.com/v1` | `.../v2` | both hosts answer (probed 2026-08-29: `/v1/` → 400, `/v2/` → 429), so v1 is still served, but v2 is what the provider documents |
| VAT Validation | `/validate`, `/rates`, `/calculate` | `/validate`, `/calculate`, `/categories` | **provider is right**: probed 2026-08-29, `vat.abstractapi.com/v1/rates` returns **404** while `/categories` returns **301**. The AE-authored `getVATRates` operation describes an endpoint that does not exist. |
| Image Processing | `/url` | `/url`, `/upload` | provider surface is larger |
| IP Geolocation | present (`ipgeolocation.abstractapi.com/v1`) | **absent** | Abstract publishes no spec for its IP Geolocation product |
| Email Validation | absent | absent | only Email *Reputation* is specified upstream |

**Upstream's own caveat**, quoted from `UPSTREAM-README.md`: only the Email Reputation spec is
"verified against the live production API"; the other twelve are "generated from the official
documentation" with nullability and exact 422/429/500 error strings "assumed generously and
pending production confirmation."

Nothing in this directory has been edited. These are archive copies for a later refine pass.

**Probe log (2026-08-29).**

| URL | Status |
|---|---|
| `https://raw.githubusercontent.com/abstractapi/openapi-specs/main/<13 files>` | 200 (all) |
| `https://companyenrichment.abstractapi.com/v1/` | 400 |
| `https://companyenrichment.abstractapi.com/v2/` | 429 |
| `https://vat.abstractapi.com/v1/rates` | 404 |
| `https://vat.abstractapi.com/v1/categories` | 301 |
| `https://images.abstractapi.com/v1/upload` | 301 |
