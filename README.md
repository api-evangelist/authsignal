# Authsignal (authsignal)

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

Authsignal is a passwordless, step-up, and risk-based authentication platform. The product wraps passkeys, authenticator apps (TOTP), SMS and WhatsApp OTP, email OTP and magic links, push notifications, biometrics (face / palm), and ID verification behind a unified Server API, Client API, and Management API. A no-code rules engine routes high-risk events through step-up challenges, and audit / observability surfaces every authentication attempt. Authsignal slots in front of existing identity providers (Cognito, Auth0, Azure AD B2C, Keycloak, IdentityServer, NextAuth.js) or works standalone.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/apis.yml)

## Tags

- Authentication
- Passkeys
- MFA
- Step-Up
- Passwordless
- Risk
- Biometrics
- Identity Verification

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Authsignal Server API

Server-to-server REST API used to track user actions, evaluate the rules engine, mint short-lived URLs for the pre-built authentication UI, issue client tokens, validate challenge results, and manage enrolled authenticators on behalf of users. Authenticated with the tenant secret (HTTP Basic with the tenant ID as username).

- **Human URL:** [https://docs.authsignal.com/api-reference/server-api/overview](https://docs.authsignal.com/api-reference/server-api/overview)
- **Base URL:** `https://api.authsignal.com`

#### Tags

- REST
- Server
- Actions
- Users
- Authenticators

#### Properties

- [Documentation](https://docs.authsignal.com/api-reference/server-api/overview)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Client API

Browser / device-facing REST API for fully custom authentication UIs. Supports passkeys, authenticator apps, SMS / WhatsApp OTP, email OTP, magic links, and push challenges. Authenticated with short-lived client tokens issued by the Server API.

- **Human URL:** [https://docs.authsignal.com/api-reference/client-api/overview](https://docs.authsignal.com/api-reference/client-api/overview)
- **Base URL:** `https://api.authsignal.com`

#### Tags

- REST
- Client
- Passkeys
- OTP

#### Properties

- [Documentation](https://docs.authsignal.com/api-reference/client-api/overview)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Management API

REST API for tenant-level configuration: actions and rules, theme and branding, and other tenant settings. Authenticated with a separate management API key.

- **Human URL:** [https://docs.authsignal.com/api-reference/management-api/overview](https://docs.authsignal.com/api-reference/management-api/overview)
- **Base URL:** `https://api.authsignal.com`

#### Tags

- REST
- Management
- Configuration
- Tenant

#### Properties

- [Documentation](https://docs.authsignal.com/api-reference/management-api/overview)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Webhooks

Outbound webhooks delivering authentication and enrollment events, enabling downstream systems to react to user lifecycle changes and challenge outcomes.

- **Human URL:** [https://docs.authsignal.com/concepts/webhooks](https://docs.authsignal.com/concepts/webhooks)
- **Base URL:** `customer-configured`

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://docs.authsignal.com/concepts/webhooks)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Node.js SDK

Official server-side SDK for Node.js / TypeScript wrapping the Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-node](https://github.com/authsignal/authsignal-node)
- **Base URL:** `https://github.com/authsignal/authsignal-node`

#### Tags

- SDK
- Node.js
- TypeScript
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-node)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Python SDK

Official server-side Python SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-python](https://github.com/authsignal/authsignal-python)
- **Base URL:** `https://github.com/authsignal/authsignal-python`

#### Tags

- SDK
- Python
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-python)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Java SDK

Official Java / Kotlin SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-java](https://github.com/authsignal/authsignal-java)
- **Base URL:** `https://github.com/authsignal/authsignal-java`

#### Tags

- SDK
- Java
- Kotlin
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-java)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal .NET SDK

Official C# / .NET SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-dotnet](https://github.com/authsignal/authsignal-dotnet)
- **Base URL:** `https://github.com/authsignal/authsignal-dotnet`

#### Tags

- SDK
- .NET
- C#
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-dotnet)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Ruby SDK

Official Ruby SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-ruby](https://github.com/authsignal/authsignal-ruby)
- **Base URL:** `https://github.com/authsignal/authsignal-ruby`

#### Tags

- SDK
- Ruby
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-ruby)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal PHP SDK

Official PHP SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-php](https://github.com/authsignal/authsignal-php)
- **Base URL:** `https://github.com/authsignal/authsignal-php`

#### Tags

- SDK
- PHP
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-php)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Go SDK

Official Go SDK for the Authsignal Server API.

- **Human URL:** [https://github.com/authsignal/authsignal-go](https://github.com/authsignal/authsignal-go)
- **Base URL:** `https://github.com/authsignal/authsignal-go`

#### Tags

- SDK
- Go
- Server

#### Properties

- [Repository](https://github.com/authsignal/authsignal-go)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Browser SDK

JavaScript / TypeScript browser SDK wrapping the Client API and WebAuthn / passkey ceremonies for web applications.

- **Human URL:** [https://github.com/authsignal/authsignal-browser](https://github.com/authsignal/authsignal-browser)
- **Base URL:** `https://github.com/authsignal/authsignal-browser`

#### Tags

- SDK
- JavaScript
- Browser
- Passkeys

#### Properties

- [Repository](https://github.com/authsignal/authsignal-browser)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal iOS SDK

Native iOS (Swift) SDK for passkeys, push, and OTP challenges in iOS applications.

- **Human URL:** [https://github.com/authsignal/authsignal-ios](https://github.com/authsignal/authsignal-ios)
- **Base URL:** `https://github.com/authsignal/authsignal-ios`

#### Tags

- SDK
- iOS
- Mobile
- Passkeys

#### Properties

- [Repository](https://github.com/authsignal/authsignal-ios)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Android SDK

Native Android (Kotlin) SDK for passkeys, push, and OTP challenges in Android applications.

- **Human URL:** [https://github.com/authsignal/authsignal-android](https://github.com/authsignal/authsignal-android)
- **Base URL:** `https://github.com/authsignal/authsignal-android`

#### Tags

- SDK
- Android
- Mobile
- Passkeys

#### Properties

- [Repository](https://github.com/authsignal/authsignal-android)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal React Native SDK

React Native wrapper around the iOS and Android SDKs.

- **Human URL:** [https://github.com/authsignal/react-native-authsignal](https://github.com/authsignal/react-native-authsignal)
- **Base URL:** `https://github.com/authsignal/react-native-authsignal`

#### Tags

- SDK
- React Native
- Mobile

#### Properties

- [Repository](https://github.com/authsignal/react-native-authsignal)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Authsignal Flutter SDK

Flutter (Dart) SDK wrapping the iOS and Android native SDKs.

- **Human URL:** [https://github.com/authsignal/authsignal-flutter](https://github.com/authsignal/authsignal-flutter)
- **Base URL:** `https://github.com/authsignal/authsignal-flutter`

#### Tags

- SDK
- Flutter
- Mobile

#### Properties

- [Repository](https://github.com/authsignal/authsignal-flutter)
- [Postman Collection](collections/authsignal.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/authsignal.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.authsignal.com/)
- [Documentation](https://docs.authsignal.com/)
- [Git Hub](https://github.com/authsignal)
- [Status](https://status.authsignal.com/)
- [Pricing](https://www.authsignal.com/pricing)
- [Blog](https://www.authsignal.com/blog)
- [LinkedIn](https://www.linkedin.com/company/authsignal)
- [L L Ms Txt](https://docs.authsignal.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
