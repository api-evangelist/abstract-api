---
name: Abstractapi
description: Use when integrating data validation, enrichment, and intelligence APIs into applications. Reach for this skill when building features that verify emails, phone numbers, IP addresses, or enrich company data; when implementing geolocation, exchange rates, or image generation; or when troubleshooting API authentication, rate limits, and error responses.
metadata:
    mintlify-proj: abstractapi
    version: "1.0"
---

# Abstract API Skill

## Product summary

Abstract API is a collection of RESTful JSON APIs for data validation, enrichment, and intelligence. Agents use it to verify emails, phone numbers, and IBANs; enrich company and contact data; detect fraud and security risks; and retrieve geolocation, exchange rates, and generated images. All APIs use HTTPS with TLS 1.2+, require unique API keys per API, and return JSON responses. Primary documentation: https://docs.abstractapi.com. Each API has a distinct base URL (e.g., `https://emailreputation.abstractapi.com/v1`, `https://phoneintelligence.abstractapi.com/v1`). Authentication uses query parameters or Bearer tokens. Metered billing charges per request, not per successful response.

## When to use

Reach for this skill when:
- Building email validation or reputation checking (deliverability, breach history, domain risk)
- Implementing phone number intelligence (carrier, location, VoIP detection, breach data)
- Adding IP geolocation or security checks (VPN/proxy/TOR detection, abuse scoring)
- Enriching company data from domains (headcount, revenue, industry, contact info)
- Generating avatars from names or images with customization
- Validating IBANs or VAT numbers
- Looking up timezones, holidays, or exchange rates
- Scraping web content or taking screenshots
- Troubleshooting API errors, rate limits, or quota issues
- Choosing between authentication methods (query param vs Bearer token)

## Quick reference

### API Base URLs and Endpoints

| API | Base URL | Required Params |
|-----|----------|-----------------|
| Email Reputation | `https://emailreputation.abstractapi.com/v1` | `api_key`, `email` |
| Phone Intelligence | `https://phoneintelligence.abstractapi.com/v1` | `api_key`, `phone` |
| IP Intelligence | `https://ip-intelligence.abstractapi.com/v1` | `api_key`, `ip_address` (optional) |
| Company Enrichment | `https://companyenrichment.abstractapi.com/v2` | `api_key`, `domain` |
| Avatars | `https://avatars.abstractapi.com/v1` | `api_key`, `name` |
| Exchange Rates | `https://exchangerates.abstractapi.com/v1` | `api_key`, `base` |
| IBAN Validation | `https://ibanvalidation.abstractapi.com/v1` | `api_key`, `iban` |
| VAT Validation | `https://vatvalidation.abstractapi.com/v1` | `api_key`, `vat_number` |
| Timezones | `https://timezoneapi.abstractapi.com/v1` | `api_key`, `location` |
| Holidays | `https://holidays.abstractapi.com/v1` | `api_key`, `country` |
| Web Scraping | `https://scrapeapi.abstractapi.com/v1` | `api_key`, `url` |
| Screenshot | `https://screenshot.abstractapi.com/v1` | `api_key`, `url` |

### Authentication Methods

**Query parameter (simplest):**
```
GET https://emailreputation.abstractapi.com/v1/?api_key=YOUR_KEY&email=user@example.com
```

**Bearer token header (secure, keeps key out of logs):**
```
GET https://emailreputation.abstractapi.com/v1/?email=user@example.com
Authorization: Bearer YOUR_KEY
```

**POST with form data:**
```
POST https://emailreputation.abstractapi.com/v1/
Content-Type: application/x-www-form-urlencoded

api_key=YOUR_KEY&email=user@example.com
```

**POST with JSON body (requires Bearer token):**
```
POST https://emailreputation.abstractapi.com/v1/
Authorization: Bearer YOUR_KEY
Content-Type: application/json

{"email": "user@example.com"}
```

### HTTP Status Codes

| Code | Type | Meaning |
|------|------|---------|
| 200 | OK | Request succeeded |
| 204 | OK | Success but no data (e.g., IP with no location) |
| 400 | Bad Request | Malformed request or invalid parameters |
| 401 | Unauthorized | Missing or incorrect API key |
| 422 | Quota Reached | Insufficient credits (free plans) |
| 429 | Too Many Requests | Rate limit exceeded (free: 1 req/sec) |
| 500 | Server Error | Abstract's server error |
| 503 | Unavailable | Service temporarily down |

### Common Response Fields

**Email Reputation:**
- `email_deliverability.status`: `deliverable`, `undeliverable`, `unknown`
- `email_quality.score`: 0.01–0.99 confidence
- `email_risk.address_risk_status`: `low`, `medium`, `high`
- `email_breaches.total_breaches`: count of known breaches

**Phone Intelligence:**
- `phone_validation.is_valid`: boolean
- `phone_carrier.line_type`: `mobile`, `landline`, `voip`, `toll_free`, etc.
- `phone_risk.risk_level`: `low`, `medium`, `high`
- `phone_location`: country, region, city, timezone

**IP Intelligence:**
- `security.is_vpn`, `is_proxy`, `is_tor`, `is_hosting`, `is_abuse`: booleans
- `location`: city, region, country, coordinates
- `timezone`: name, UTC offset, local time
- `asn`: Autonomous System Number and ISP info

**Company Enrichment:**
- `company_name`, `industry`, `employee_count`, `annual_revenue`
- `logo`, `phone_numbers`, `email_addresses`
- `linkedin_url`, `facebook_url`, `twitter_url`, etc.

### Field Filtering

Some APIs support limiting response fields with a `fields` parameter:
```
GET https://ip-intelligence.abstractapi.com/v1/?api_key=KEY&ip_address=1.2.3.4&fields=country,city
```

## Decision guidance

### When to use query parameter vs Bearer token authentication

| Scenario | Use |
|----------|-----|
| Simple scripts, testing, curl commands | Query parameter (`?api_key=...`) |
| Production code, server logs, security-sensitive | Bearer token header |
| Bulk processing, many requests | POST with form data or JSON |
| Sensitive environments (logs visible to others) | Bearer token only |

### When to use GET vs POST

| Scenario | Use |
|----------|-----|
| Single request, simple parameters | GET |
| Sensitive data (e.g., email in URL logs) | POST with Bearer token |
| Bulk operations, many parameters | POST with JSON body |
| API key in URL is acceptable | GET |

### When to filter response fields

| Scenario | Use |
|----------|-----|
| Need all data for analysis | Full response (no `fields` param) |
| Bandwidth-constrained, only need subset | `fields=country,city` |
| Parsing specific fields in code | Full response (easier to handle) |
| Reducing payload size | `fields=` parameter |

## Workflow

1. **Identify the API needed**: Determine which Abstract API solves the problem (email validation, phone lookup, IP geolocation, etc.).

2. **Obtain the API key**: Retrieve the unique API key for that specific API from the Abstract dashboard. Note: each API has its own key.

3. **Choose authentication method**: Decide between query parameter (simple) or Bearer token (secure). For production, prefer Bearer token.

4. **Construct the request**: Build the URL or POST body with required parameters (`api_key`, primary parameter like `email`/`phone`/`ip_address`/`domain`). Add optional parameters (e.g., `fields` for filtering, `country` for phone numbers).

5. **Make the request**: Send GET or POST request to the API's base URL. Ensure HTTPS and TLS 1.2+.

6. **Handle the response**: Parse JSON response. Check HTTP status code first:
   - 200/204: Success. Extract data from response fields.
   - 401: API key missing or wrong. Verify key and authentication method.
   - 422: Out of credits. Check account quota.
   - 429: Rate limit hit. Implement backoff (free plans: 1 req/sec max).
   - 400/500/503: Validate request format or retry later.

7. **Verify results**: Check response fields for expected data. For validation APIs (email, phone, IBAN), check the `is_valid` or `status` field. For enrichment APIs, confirm required fields are present.

8. **Handle null/missing fields**: Some fields return `null` if data unavailable. Plan for this in code (e.g., email format invalid → quality fields are null).

## Common gotchas

- **Each API has a unique key**: Email Reputation API key won't work for Phone Intelligence API. Verify you're using the correct key for the endpoint.

- **Metered billing charges per request, not per success**: Invalid requests (e.g., malformed email, fake IP) still consume credits. Test with valid data first.

- **API key in query parameter appears in logs**: Use Bearer token header in production to keep keys out of server logs and URLs.

- **Free plans limited to 1 request per second**: 429 errors occur if you exceed this. Implement rate limiting on client side (queue requests, add delays).

- **Free plans have quota limits**: 422 error means you've exhausted credits. Check account dashboard for remaining quota.

- **IP address auto-detection without parameter**: If you omit `ip_address` in IP Intelligence API, it geolocates the request origin IP. Explicitly pass `ip_address` to analyze a specific IP.

- **Phone number country code matters**: Phone Intelligence API may need `country` parameter to correctly parse numbers. Always include it if number format is ambiguous.

- **Email format validation fails silently**: If email format is invalid, other checks (SMTP, MX, quality) return `null` or `false`. Check `is_format_valid` first.

- **Domain vs email in Company Enrichment**: API requires domain (e.g., `airbnb.com`), not email. Extract domain from email if needed.

- **Bearer token format**: Use `Authorization: Bearer YOUR_KEY`, not `Authorization: YOUR_KEY` or `Authorization: ApiKey YOUR_KEY`.

- **POST with JSON requires Content-Type header**: Omitting `Content-Type: application/json` causes body to be read as form data, and parameters won't be detected.

- **Null vs missing fields**: Some APIs return `null` for unavailable data; others omit the field. Handle both cases in parsing.

- **Rate limit applies per second, not per minute**: Free plans reset every second, not every 60 seconds. Spread requests across time.

## Verification checklist

Before submitting work with Abstract API:

- [ ] Correct API key is used for the target API (not a key from a different API)
- [ ] Required parameters are present and valid (e.g., email format, valid IP, domain without `http://`)
- [ ] Authentication method is correct (query param or Bearer token header)
- [ ] HTTPS is used (not HTTP)
- [ ] HTTP status code is checked before parsing response
- [ ] Response fields are checked for `null` values before use
- [ ] Rate limiting is implemented (free: max 1 req/sec)
- [ ] Error handling covers 401 (auth), 422 (quota), 429 (rate limit), 400 (bad request), 500/503 (server)
- [ ] Sensitive data (API keys) not logged or exposed in URLs (use Bearer token)
- [ ] POST requests with JSON include `Content-Type: application/json` header
- [ ] Field filtering (`fields` parameter) is used only if bandwidth is constrained
- [ ] Bulk CSV uploads respect 50,000 row limit and proper formatting
- [ ] Response parsing handles both present and absent optional fields

## Resources

- **Full API documentation and page listing**: https://docs.abstractapi.com/llms.txt
- **Email Reputation API**: https://docs.abstractapi.com/api/email-reputation
- **Phone Intelligence API**: https://docs.abstractapi.com/api/phone-intelligence
- **IP Intelligence API**: https://docs.abstractapi.com/api/ip-intelligence

---

> For additional documentation and navigation, see: https://docs.abstractapi.com/llms.txt