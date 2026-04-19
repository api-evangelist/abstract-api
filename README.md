# Abstract API (abstract-api)
Abstract API is a platform that offers a wide range of API services for developers to easily integrate various functionalities into their applications. Services include IP geolocation, IP intelligence, email validation, phone validation, currency exchange, website screenshots, image processing, web scraping, company enrichment, public holidays, timezone lookup, VAT validation, IBAN validation, and user avatar generation. Abstract API provides a seamless way for developers to access powerful features without having to build them from scratch.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Avatars, Company Enrichment, Contacts, Currencies, Email Validation, Exchange Rates, IBAN Validation, Image Processing, IP Geolocation, IP Intelligence, Phone Validation, Public Holidays, Screenshots, Timezones, VAT Validation, Web Scraping

## Timestamps

- **Created:** 2025-02-24
- **Modified:** 2026-04-19

## APIs

### Email Reputation API
Validate email addresses for deliverability, detect disposable or risky domains, verify SMTP/MX records, and enrich email data with sender information, breach history, and risk scoring.

**Human URL:** [https://www.abstractapi.com/api/email-verification-validation-api](https://www.abstractapi.com/api/email-verification-validation-api)

#### Tags:

 - Email Validation, Email Reputation, Fraud Detection

#### Properties

- [Documentation](https://docs.abstractapi.com/api/email-reputation.md)
- [OpenAPI](openapi/abstract-api-email-reputation.yaml)
- [JSONSchema](json-schema/email-reputation-breach-info-schema.json)
- [Example](examples/email-reputation-breach-info-example.json)

### Phone Intelligence API
Identify carrier, line type, validity, location, and get deep insights including line status, VoIP detection, and risk scoring for any phone number globally.

**Human URL:** [https://www.abstractapi.com/api/phone-validation-api](https://www.abstractapi.com/api/phone-validation-api)

#### Tags:

 - Phone Validation, Phone Intelligence, Fraud Detection

#### Properties

- [Documentation](https://docs.abstractapi.com/api/phone-intelligence.md)
- [OpenAPI](openapi/abstract-api-phone-intelligence.yaml)
- [JSONSchema](json-schema/phone-intelligence-phone-country-schema.json)
- [Example](examples/phone-intelligence-phone-country-example.json)

### IP Geolocation API
Geolocate any IPv4 or IPv6 address to country, region, city, coordinates, timezone, currency, and flag data covering 4 billion+ IP addresses across 250,000+ cities worldwide.

**Human URL:** [https://www.abstractapi.com/api/ip-geolocation-api](https://www.abstractapi.com/api/ip-geolocation-api)

#### Tags:

 - IP Geolocation, IP Addresses, Geolocation

#### Properties

- [Documentation](https://www.abstractapi.com/api/ip-geolocation-api)
- [OpenAPI](openapi/abstract-api-ip-geolocation.yaml)
- [JSONSchema](json-schema/ip-geolocation-currency-info-schema.json)
- [Example](examples/ip-geolocation-currency-info-example.json)

### IP Intelligence API
Detect VPNs, proxies, Tor exit nodes, abuse potential, hosting services, relays, and mobile IPs. Also provides ASN, company, location, timezone, flag, and currency data for any IP address.

**Human URL:** [https://www.abstractapi.com/api/ip-intelligence](https://www.abstractapi.com/api/ip-intelligence)

#### Tags:

 - IP Intelligence, IP Addresses, Security, Fraud Detection

#### Properties

- [Documentation](https://docs.abstractapi.com/api/ip-intelligence.md)
- [OpenAPI](openapi/abstract-api-ip-intelligence.yaml)
- [JSONSchema](json-schema/ip-intelligence-asn-info-schema.json)
- [Example](examples/ip-intelligence-asn-info-example.json)

### Company Enrichment API
Retrieve comprehensive details about businesses using their domain or email address, including name, logo, headcount, location, industry, and more.

**Human URL:** [https://www.abstractapi.com/api/company-enrichment](https://www.abstractapi.com/api/company-enrichment)

#### Tags:

 - Company Enrichment, Business Data, Data Enrichment

#### Properties

- [Documentation](https://docs.abstractapi.com/api/company-enrichment.md)
- [OpenAPI](openapi/abstract-api-company-enrichment.yaml)
- [JSONSchema](json-schema/company-enrichment-company-enrichment-response-schema.json)
- [Example](examples/company-enrichment-company-enrichment-response-example.json)

### Exchange Rates API
Look up the latest exchange rates for 80+ currencies, convert between currencies, and retrieve historical exchange rate data using ISO 4217 currency codes.

**Human URL:** [https://www.abstractapi.com/api/exchange-rate-api](https://www.abstractapi.com/api/exchange-rate-api)

#### Tags:

 - Currencies, Exchange Rates, Finance

#### Properties

- [Documentation](https://docs.abstractapi.com/api/exchange-rates.md)
- [OpenAPI](openapi/abstract-api-exchange-rates.yaml)
- [JSONSchema](json-schema/exchange-rates-convert-response-schema.json)
- [Example](examples/exchange-rates-convert-response-example.json)

### Public Holidays API
Get public, local, religious, and other holidays for any country. Supports year and country filtering with comprehensive holiday metadata.

**Human URL:** [https://www.abstractapi.com/api/holidays-api](https://www.abstractapi.com/api/holidays-api)

#### Tags:

 - Public Holidays, Calendar, Global Data

#### Properties

- [Documentation](https://docs.abstractapi.com/api/holidays.md)
- [OpenAPI](openapi/abstract-api-public-holidays.yaml)
- [JSONSchema](json-schema/public-holidays-holiday-schema.json)
- [Example](examples/public-holidays-holiday-example.json)

### Timezone API
Find, convert, and manage time and timezone data across the world. Supports lookup by location or coordinates and returns local time, timezone abbreviation, UTC offset, and DST information.

**Human URL:** [https://www.abstractapi.com/api/time-date-timezone-api](https://www.abstractapi.com/api/time-date-timezone-api)

#### Tags:

 - Timezones, Time, Date, Calendar

#### Properties

- [Documentation](https://docs.abstractapi.com/api/timezones.md)
- [OpenAPI](openapi/abstract-api-timezones.yaml)
- [JSONSchema](json-schema/timezones-convert-time-response-schema.json)
- [Example](examples/timezones-convert-time-response-example.json)

### VAT Validation API
Validate VAT numbers, look up current VAT rates by country, and calculate VAT-inclusive or VAT-exclusive prices to stay compliant for domestic and cross-border sales.

**Human URL:** [https://www.abstractapi.com/api/vat-validation-rates-api](https://www.abstractapi.com/api/vat-validation-rates-api)

#### Tags:

 - VAT Validation, Finance, Compliance, Tax

#### Properties

- [Documentation](https://docs.abstractapi.com/api/vat-validation.md)
- [OpenAPI](openapi/abstract-api-vat-validation.yaml)
- [JSONSchema](json-schema/vat-validation-vat-calculate-response-schema.json)
- [Example](examples/vat-validation-vat-calculate-response-example.json)

### IBAN Validation API
Determine the validity and details of International Bank Account Numbers (IBANs), including bank name, account type, and country code.

**Human URL:** [https://www.abstractapi.com/api/iban-validation](https://www.abstractapi.com/api/iban-validation)

#### Tags:

 - IBAN Validation, Finance, Banking

#### Properties

- [Documentation](https://docs.abstractapi.com/api/iban-validation.md)
- [OpenAPI](openapi/abstract-api-iban-validation.yaml)
- [JSONSchema](json-schema/iban-validation-iban-validation-response-schema.json)
- [Example](examples/iban-validation-iban-validation-response-example.json)

### Website Screenshot API
Capture high-quality screenshots of any website with optional customizations including CSS injection, delay settings, and viewport configuration.

**Human URL:** [https://www.abstractapi.com/api/website-screenshot-api](https://www.abstractapi.com/api/website-screenshot-api)

#### Tags:

 - Screenshots, Web Capture, Images

#### Properties

- [Documentation](https://docs.abstractapi.com/api/screenshot.md)
- [OpenAPI](openapi/abstract-api-website-screenshot.yaml)

### Image Processing API
Compress, convert, and optimize images by URL or direct upload. Supports format conversion, quality adjustment, and size reduction.

**Human URL:** [https://www.abstractapi.com/api/image-processing-optimization-api](https://www.abstractapi.com/api/image-processing-optimization-api)

#### Tags:

 - Image Processing, Images, Optimization

#### Properties

- [Documentation](https://docs.abstractapi.com/api/images.md)
- [OpenAPI](openapi/abstract-api-image-processing.yaml)
- [JSONSchema](json-schema/image-processing-image-processing-response-schema.json)
- [Example](examples/image-processing-image-processing-response-example.json)

### Web Scraping API
Extract data from any website by providing the target URL. Handles JavaScript rendering and returns the full HTML content of any web page.

**Human URL:** [https://www.abstractapi.com/api/web-scraping-api](https://www.abstractapi.com/api/web-scraping-api)

#### Tags:

 - Web Scraping, Data Extraction, HTML

#### Properties

- [Documentation](https://docs.abstractapi.com/api/scrape.md)
- [OpenAPI](openapi/abstract-api-web-scraping.yaml)
- [JSONSchema](json-schema/web-scraping-web-scraping-response-schema.json)
- [Example](examples/web-scraping-web-scraping-response-example.json)

### Avatars API
Create highly customizable avatar images using a person's name or initials. Supports color, font, and size customization for user profile images.

**Human URL:** [https://www.abstractapi.com/api/user-avatar-api](https://www.abstractapi.com/api/user-avatar-api)

#### Tags:

 - Avatars, Images, User Interface

#### Properties

- [Documentation](https://docs.abstractapi.com/api/avatars.md)
- [OpenAPI](openapi/abstract-api-avatars.yaml)

## Common Properties

- [Website](https://www.abstractapi.com/)
- [Portal](https://app.abstractapi.com/)
- [SignUp](https://app.abstractapi.com/users/signup)
- [Login](https://app.abstractapi.com/users/login)
- [Pricing](https://www.abstractapi.com/pricing)
- [Blog](https://www.abstractapi.com/blog)
- [Documentation](https://docs.abstractapi.com/)
- [GettingStarted](https://docs.abstractapi.com/)
- [GitHubOrganization](https://github.com/abstractapi)
- [TermsOfService](https://www.abstractapi.com/legal/terms)
- [PrivacyPolicy](https://www.abstractapi.com/legal/privacy)
- [SpectralRules](rules/abstract-api-spectral-rules.yml)
- [NaftikoCapability](capabilities/fraud-detection.yaml)
- [NaftikoCapability](capabilities/data-enrichment.yaml)
- [NaftikoCapability](capabilities/financial-compliance.yaml)
- [Vocabulary](vocabulary/abstract-api-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| API Key Authentication | Each API uses a unique API key passed as a query parameter or Bearer token header |
| Free Tier | Each API offers a free tier with limited monthly requests and 1 request/second rate limit |
| Simple REST API | All APIs follow a simple REST pattern with a single base URL and query parameters |
| Global Coverage | Data covers global locations with 80+ currencies, 250,000+ cities, and worldwide phone/IP coverage |
| JSON Responses | All API responses return structured JSON data with consistent error codes |
| Modular Services | Each API is independently keyed and priced, allowing granular subscription management |

## Use Cases

| Name | Description |
|------|-------------|
| Email List Cleaning | Validate and filter email lists to improve deliverability and reduce bounce rates |
| Fraud Detection | Use IP intelligence, email reputation, and phone intelligence to detect and block fraudulent users |
| User Onboarding Enrichment | Automatically enrich user profiles with geolocation, company, and contact data at signup |
| Currency Conversion | Display localized pricing or perform currency conversions in e-commerce and fintech apps |
| Compliance Automation | Validate VAT numbers and IBAN codes to automate financial compliance workflows |
| Content Extraction | Use web scraping API to extract structured data from any website for data pipelines |
| Dynamic User Avatars | Generate placeholder avatars for users without profile photos using the Avatars API |

## Integrations

| Name | Description |
|------|-------------|
| JavaScript | Official JavaScript SDK for Exchange Rates, Email Validation, IP Geolocation, and Phone Validation |
| Python | Official Python SDK for Exchange Rates, Email Validation, IP Geolocation, and Phone Validation |
| PHP | Official PHP SDK for Exchange Rates, Email Validation, IP Geolocation, and Phone Validation |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Abstract Api Avatars](openapi/abstract-api-avatars.yaml)
- [Abstract Api Company Enrichment](openapi/abstract-api-company-enrichment.yaml)
- [Abstract Api Email Reputation](openapi/abstract-api-email-reputation.yaml)
- [Abstract Api Exchange Rates](openapi/abstract-api-exchange-rates.yaml)
- [Abstract Api Iban Validation](openapi/abstract-api-iban-validation.yaml)
- [Abstract Api Image Processing](openapi/abstract-api-image-processing.yaml)
- [Abstract Api Ip Geolocation](openapi/abstract-api-ip-geolocation.yaml)
- [Abstract Api Ip Intelligence](openapi/abstract-api-ip-intelligence.yaml)
- [Abstract Api Phone Intelligence](openapi/abstract-api-phone-intelligence.yaml)
- [Abstract Api Public Holidays](openapi/abstract-api-public-holidays.yaml)
- [Abstract Api Timezones](openapi/abstract-api-timezones.yaml)
- [Abstract Api Vat Validation](openapi/abstract-api-vat-validation.yaml)
- [Abstract Api Web Scraping](openapi/abstract-api-web-scraping.yaml)
- [Abstract Api Website Screenshot](openapi/abstract-api-website-screenshot.yaml)

### JSON Schema

- [Company Enrichment Company Enrichment Response](json-schema/company-enrichment-company-enrichment-response-schema.json)
- [Email Reputation Breach Info](json-schema/email-reputation-breach-info-schema.json)
- [Email Reputation Deliverability](json-schema/email-reputation-deliverability-schema.json)
- [Email Reputation Domain Info](json-schema/email-reputation-domain-info-schema.json)
- [Email Reputation Email Quality](json-schema/email-reputation-email-quality-schema.json)
- [Email Reputation Email Reputation Response](json-schema/email-reputation-email-reputation-response-schema.json)
- [Email Reputation Risk Info](json-schema/email-reputation-risk-info-schema.json)
- [Email Reputation Sender Info](json-schema/email-reputation-sender-info-schema.json)
- [Exchange Rates Convert Response](json-schema/exchange-rates-convert-response-schema.json)
- [Exchange Rates Historical Rates Response](json-schema/exchange-rates-historical-rates-response-schema.json)
- [Exchange Rates Live Rates Response](json-schema/exchange-rates-live-rates-response-schema.json)
- [Iban Validation Iban Validation Response](json-schema/iban-validation-iban-validation-response-schema.json)
- [Image Processing Image Processing Response](json-schema/image-processing-image-processing-response-schema.json)
- [Ip Geolocation Currency Info](json-schema/ip-geolocation-currency-info-schema.json)
- [Ip Geolocation Flag Info](json-schema/ip-geolocation-flag-info-schema.json)
- [Ip Geolocation Ip Geolocation Response](json-schema/ip-geolocation-ip-geolocation-response-schema.json)
- [Ip Geolocation Security Info](json-schema/ip-geolocation-security-info-schema.json)
- [Ip Geolocation Timezone Info](json-schema/ip-geolocation-timezone-info-schema.json)
- [Ip Intelligence Asn Info](json-schema/ip-intelligence-asn-info-schema.json)
- [Ip Intelligence Company Basic](json-schema/ip-intelligence-company-basic-schema.json)
- [Ip Intelligence Currency Info](json-schema/ip-intelligence-currency-info-schema.json)
- [Ip Intelligence Flag Info](json-schema/ip-intelligence-flag-info-schema.json)
- [Ip Intelligence Ip Intelligence Response](json-schema/ip-intelligence-ip-intelligence-response-schema.json)
- [Ip Intelligence Ip Security Flags](json-schema/ip-intelligence-ip-security-flags-schema.json)
- [Ip Intelligence Location Info](json-schema/ip-intelligence-location-info-schema.json)
- [Ip Intelligence Timezone Info](json-schema/ip-intelligence-timezone-info-schema.json)
- [Phone Intelligence Phone Country](json-schema/phone-intelligence-phone-country-schema.json)
- [Phone Intelligence Phone Intelligence Response](json-schema/phone-intelligence-phone-intelligence-response-schema.json)
- [Public Holidays Holiday](json-schema/public-holidays-holiday-schema.json)
- [Timezones Convert Time Response](json-schema/timezones-convert-time-response-schema.json)
- [Timezones Current Time Response](json-schema/timezones-current-time-response-schema.json)
- [Vat Validation Vat Calculate Response](json-schema/vat-validation-vat-calculate-response-schema.json)
- [Vat Validation Vat Rates Response](json-schema/vat-validation-vat-rates-response-schema.json)
- [Vat Validation Vat Validation Response](json-schema/vat-validation-vat-validation-response-schema.json)
- [Web Scraping Web Scraping Response](json-schema/web-scraping-web-scraping-response-schema.json)

### JSON Structure

- [Company Enrichment Company Enrichment Response](json-structure/company-enrichment-company-enrichment-response-structure.json)
- [Email Reputation Breach Info](json-structure/email-reputation-breach-info-structure.json)
- [Email Reputation Deliverability](json-structure/email-reputation-deliverability-structure.json)
- [Email Reputation Domain Info](json-structure/email-reputation-domain-info-structure.json)
- [Email Reputation Email Quality](json-structure/email-reputation-email-quality-structure.json)
- [Email Reputation Email Reputation Response](json-structure/email-reputation-email-reputation-response-structure.json)
- [Email Reputation Risk Info](json-structure/email-reputation-risk-info-structure.json)
- [Email Reputation Sender Info](json-structure/email-reputation-sender-info-structure.json)
- [Exchange Rates Convert Response](json-structure/exchange-rates-convert-response-structure.json)
- [Exchange Rates Historical Rates Response](json-structure/exchange-rates-historical-rates-response-structure.json)
- [Exchange Rates Live Rates Response](json-structure/exchange-rates-live-rates-response-structure.json)
- [Iban Validation Iban Validation Response](json-structure/iban-validation-iban-validation-response-structure.json)
- [Image Processing Image Processing Response](json-structure/image-processing-image-processing-response-structure.json)
- [Ip Geolocation Currency Info](json-structure/ip-geolocation-currency-info-structure.json)
- [Ip Geolocation Flag Info](json-structure/ip-geolocation-flag-info-structure.json)
- [Ip Geolocation Ip Geolocation Response](json-structure/ip-geolocation-ip-geolocation-response-structure.json)
- [Ip Geolocation Security Info](json-structure/ip-geolocation-security-info-structure.json)
- [Ip Geolocation Timezone Info](json-structure/ip-geolocation-timezone-info-structure.json)
- [Ip Intelligence Asn Info](json-structure/ip-intelligence-asn-info-structure.json)
- [Ip Intelligence Company Basic](json-structure/ip-intelligence-company-basic-structure.json)
- [Ip Intelligence Currency Info](json-structure/ip-intelligence-currency-info-structure.json)
- [Ip Intelligence Flag Info](json-structure/ip-intelligence-flag-info-structure.json)
- [Ip Intelligence Ip Intelligence Response](json-structure/ip-intelligence-ip-intelligence-response-structure.json)
- [Ip Intelligence Ip Security Flags](json-structure/ip-intelligence-ip-security-flags-structure.json)
- [Ip Intelligence Location Info](json-structure/ip-intelligence-location-info-structure.json)
- [Ip Intelligence Timezone Info](json-structure/ip-intelligence-timezone-info-structure.json)
- [Phone Intelligence Phone Country](json-structure/phone-intelligence-phone-country-structure.json)
- [Phone Intelligence Phone Intelligence Response](json-structure/phone-intelligence-phone-intelligence-response-structure.json)
- [Public Holidays Holiday](json-structure/public-holidays-holiday-structure.json)
- [Timezones Convert Time Response](json-structure/timezones-convert-time-response-structure.json)
- [Timezones Current Time Response](json-structure/timezones-current-time-response-structure.json)
- [Vat Validation Vat Calculate Response](json-structure/vat-validation-vat-calculate-response-structure.json)
- [Vat Validation Vat Rates Response](json-structure/vat-validation-vat-rates-response-structure.json)
- [Vat Validation Vat Validation Response](json-structure/vat-validation-vat-validation-response-structure.json)
- [Web Scraping Web Scraping Response](json-structure/web-scraping-web-scraping-response-structure.json)

### JSON-LD

- [Abstract Api Company Enrichment](json-ld/abstract-api-company-enrichment-context.jsonld)
- [Abstract Api Email Reputation](json-ld/abstract-api-email-reputation-context.jsonld)
- [Abstract Api Exchange Rates](json-ld/abstract-api-exchange-rates-context.jsonld)
- [Abstract Api Iban Validation](json-ld/abstract-api-iban-validation-context.jsonld)
- [Abstract Api Image Processing](json-ld/abstract-api-image-processing-context.jsonld)
- [Abstract Api Ip Geolocation](json-ld/abstract-api-ip-geolocation-context.jsonld)
- [Abstract Api Ip Intelligence](json-ld/abstract-api-ip-intelligence-context.jsonld)
- [Abstract Api Phone Intelligence](json-ld/abstract-api-phone-intelligence-context.jsonld)
- [Abstract Api Public Holidays](json-ld/abstract-api-public-holidays-context.jsonld)
- [Abstract Api Timezones Convert](json-ld/abstract-api-timezones-convert-context.jsonld)
- [Abstract Api Timezones Current](json-ld/abstract-api-timezones-current-context.jsonld)
- [Abstract Api Vat Validation](json-ld/abstract-api-vat-validation-context.jsonld)
- [Abstract Api Web Scraping](json-ld/abstract-api-web-scraping-context.jsonld)

### Examples

- [Company Enrichment Company Enrichment Response](examples/company-enrichment-company-enrichment-response-example.json)
- [Email Reputation Breach Info](examples/email-reputation-breach-info-example.json)
- [Email Reputation Deliverability](examples/email-reputation-deliverability-example.json)
- [Email Reputation Domain Info](examples/email-reputation-domain-info-example.json)
- [Email Reputation Email Quality](examples/email-reputation-email-quality-example.json)
- [Email Reputation Email Reputation Response](examples/email-reputation-email-reputation-response-example.json)
- [Email Reputation Risk Info](examples/email-reputation-risk-info-example.json)
- [Email Reputation Sender Info](examples/email-reputation-sender-info-example.json)
- [Exchange Rates Convert Response](examples/exchange-rates-convert-response-example.json)
- [Exchange Rates Historical Rates Response](examples/exchange-rates-historical-rates-response-example.json)
- [Exchange Rates Live Rates Response](examples/exchange-rates-live-rates-response-example.json)
- [Iban Validation Iban Validation Response](examples/iban-validation-iban-validation-response-example.json)
- [Image Processing Image Processing Response](examples/image-processing-image-processing-response-example.json)
- [Ip Geolocation Currency Info](examples/ip-geolocation-currency-info-example.json)
- [Ip Geolocation Flag Info](examples/ip-geolocation-flag-info-example.json)
- [Ip Geolocation Ip Geolocation Response](examples/ip-geolocation-ip-geolocation-response-example.json)
- [Ip Geolocation Security Info](examples/ip-geolocation-security-info-example.json)
- [Ip Geolocation Timezone Info](examples/ip-geolocation-timezone-info-example.json)
- [Ip Intelligence Asn Info](examples/ip-intelligence-asn-info-example.json)
- [Ip Intelligence Company Basic](examples/ip-intelligence-company-basic-example.json)
- [Ip Intelligence Currency Info](examples/ip-intelligence-currency-info-example.json)
- [Ip Intelligence Flag Info](examples/ip-intelligence-flag-info-example.json)
- [Ip Intelligence Ip Intelligence Response](examples/ip-intelligence-ip-intelligence-response-example.json)
- [Ip Intelligence Ip Security Flags](examples/ip-intelligence-ip-security-flags-example.json)
- [Ip Intelligence Location Info](examples/ip-intelligence-location-info-example.json)
- [Ip Intelligence Timezone Info](examples/ip-intelligence-timezone-info-example.json)
- [Phone Intelligence Phone Country](examples/phone-intelligence-phone-country-example.json)
- [Phone Intelligence Phone Intelligence Response](examples/phone-intelligence-phone-intelligence-response-example.json)
- [Public Holidays Holiday](examples/public-holidays-holiday-example.json)
- [Timezones Convert Time Response](examples/timezones-convert-time-response-example.json)
- [Timezones Current Time Response](examples/timezones-current-time-response-example.json)
- [Vat Validation Vat Calculate Response](examples/vat-validation-vat-calculate-response-example.json)
- [Vat Validation Vat Rates Response](examples/vat-validation-vat-rates-response-example.json)
- [Vat Validation Vat Validation Response](examples/vat-validation-vat-validation-response-example.json)
- [Web Scraping Web Scraping Response](examples/web-scraping-web-scraping-response-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Avatars](capabilities/shared/avatars.yaml)
- [Company Enrichment](capabilities/shared/company-enrichment.yaml)
- [Email Reputation](capabilities/shared/email-reputation.yaml)
- [Exchange Rates](capabilities/shared/exchange-rates.yaml)
- [Iban Validation](capabilities/shared/iban-validation.yaml)
- [Image Processing](capabilities/shared/image-processing.yaml)
- [Ip Geolocation](capabilities/shared/ip-geolocation.yaml)
- [Ip Intelligence](capabilities/shared/ip-intelligence.yaml)
- [Phone Intelligence](capabilities/shared/phone-intelligence.yaml)
- [Public Holidays](capabilities/shared/public-holidays.yaml)
- [Timezones](capabilities/shared/timezones.yaml)
- [Vat Validation](capabilities/shared/vat-validation.yaml)
- [Web Scraping](capabilities/shared/web-scraping.yaml)
- [Website Screenshot](capabilities/shared/website-screenshot.yaml)

### Workflow Capabilities

| Workflow | Description |
|----------|-------------|
| [Data Enrichment](capabilities/data-enrichment.yaml) | IP geolocation, company enrichment, and timezone data for user profile enrichment |
| [Financial Compliance](capabilities/financial-compliance.yaml) | Exchange rates, VAT validation, and IBAN validation for financial compliance |
| [Fraud Detection](capabilities/fraud-detection.yaml) | Email reputation, phone intelligence, and IP intelligence for fraud prevention |

## Vocabulary

- [Abstract Api Vocabulary](vocabulary/abstract-api-vocabulary.yaml) — Unified taxonomy mapping 13 resources, 9 actions, 3 workflows, and 6 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Abstract Api Spectral Rules](rules/abstract-api-spectral-rules.yml) — 33 rules across 13 categories enforcing Abstract API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com

