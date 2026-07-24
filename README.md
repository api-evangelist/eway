# eWAY (eway)

eWAY (Eway) is an Australian online payment gateway founded in Sydney in 1998 and now part of Global Payments Oceania, providing card-not-present payment acceptance for e-commerce merchants across Australia, New Zealand, and Asia. Its flagship developer surface is the Rapid API — a versioned HTTP payments API (currently version 47) that processes purchases, pre-authorisations, MOTO and recurring transactions, and tokenised (stored-card) payments through seven integration methods, from server-to-server Direct Connection to PCI-scope-reducing Transparent Redirect, Secure Fields, and the Responsive Shared Page.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/eway/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/eway/refs/heads/main/apis.yml)

## Tags

- Payments
- Australia
- Payment Gateway
- Payment Processing
- Card Payments
- Tokenization
- E-commerce
- Recurring Payments
- Subscriptions

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

### eWAY Rapid API

The eWAY Rapid API is a versioned HTTP payments API (v47) for processing card transactions. It exposes transaction creation (Direct Connection), AccessCode-based flows (Transparent Redirect / Responsive Shared Page / Secure Fields), transaction query by ID, and token-customer, refund, and cancel-authorisation operations. It supports REST/JSON (recommended) plus SOAP, XML, and RPC formats. Authentication is HTTP Basic (API key as username, password as password) with an `X-EWAY-APIVERSION` header selecting the version.

- **Human URL:** [https://eway.io/api-v3/](https://eway.io/api-v3/)
- **Base URL (production):** `https://api.ewaypayments.com/`
- **Base URL (sandbox):** `https://api.sandbox.ewaypayments.com/`

#### Tags

- Payments
- Card Payments
- Tokenization
- Recurring Payments

#### Properties

- [Documentation](https://eway.io/api-v3/)
- [API Reference](https://eway.io/api-v3/)
- [Documentation](https://www.eway.com.au/documentation/)
- [SDKs (GitHub)](https://github.com/eWAYPayment)

## API Posture

eWAY is genuinely API-first: the Rapid API is publicly and well documented, versioned, with a free sandbox and open-source MIT-licensed SDKs (PHP, Java, .NET, .NET Standard, Node.js, Ruby, Android, iOS) under the [eWAYPayment](https://github.com/eWAYPayment) GitHub organization. However, eWAY does **not** publish a downloadable OpenAPI/Swagger definition — none was found on the docs host or the API host — so zero specs were harvested. Authentication is HTTP Basic; there is no OAuth2/OIDC, no public webhooks catalog, and no AsyncAPI event stream. As a card gateway (not an NPP account-to-account rail), there is no ISO 20022 posture.

## Common Properties

- [Website](https://www.eway.com.au/)
- [Developer Portal](https://eway.io/api-v3/)
- [Documentation](https://www.eway.com.au/documentation/)
- [API Reference](https://eway.io/api-v3/)
- [GitHub Organization](https://github.com/eWAYPayment)
- [Status Page](https://status.eway.com.au/)
- [Pricing](https://www.eway.com.au/plans-pricing/)
- [Blog](https://www.eway.com.au/blog/)
- [Support](https://www.eway.com.au/support/)
- [Sign Up](https://www.eway.com.au/sign-up/)
- [Login](https://au.myeway.com/)
- [Terms of Service](https://www.eway.com.au/legal/)
- [Privacy Policy](https://www.eway.com.au/legals/privacy-policy/)
- [Security](https://www.eway.com.au/security/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
