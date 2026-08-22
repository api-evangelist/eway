# eWAY (eway)

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
