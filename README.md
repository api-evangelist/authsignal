# Authsignal

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

**Areas:** Authentication · Passkeys · MFA · Step-Up · Passwordless · Risk Management · Biometrics · Identity Verification

## Authsignal on APIs.io

Everything profiled for Authsignal is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/authsignal/](https://apis.io/providers/authsignal/)** — or go straight to one of the APIs or properties below.

### APIs (22)

- [Authsignal Server API](https://apis.io/apis/authsignal/server-api/) — Server-to-server REST API used to track user actions, evaluate the rules engine, mint short-lived URLs for the pre-built authentication UI, issue client…
- [Authsignal Client API](https://apis.io/apis/authsignal/client-api/) — Browser / device-facing REST API for fully custom authentication UIs. Supports passkeys, authenticator apps, SMS / WhatsApp OTP, email OTP, magic links, and…
- [Authsignal Management API](https://apis.io/apis/authsignal/management-api/) — REST API for tenant-level configuration: actions and rules, theme and branding, and other tenant settings. Authenticated with a separate management API key.
- [Authsignal Webhooks](https://apis.io/apis/authsignal/webhooks/) — Outbound webhooks delivering authentication and enrollment events, enabling downstream systems to react to user lifecycle changes and challenge outcomes.
- [Authsignal Node.js SDK](https://apis.io/apis/authsignal/sdk-node/) — Official server-side SDK for Node.js / TypeScript wrapping the Server API.
- [Authsignal Python SDK](https://apis.io/apis/authsignal/sdk-python/) — Official server-side Python SDK for the Authsignal Server API.
- [Authsignal Java SDK](https://apis.io/apis/authsignal/sdk-java/) — Official Java / Kotlin SDK for the Authsignal Server API.
- [Authsignal .NET SDK](https://apis.io/apis/authsignal/sdk-dotnet/) — Official C# / .NET SDK for the Authsignal Server API.
- [Authsignal Ruby SDK](https://apis.io/apis/authsignal/sdk-ruby/) — Official Ruby SDK for the Authsignal Server API.
- [Authsignal PHP SDK](https://apis.io/apis/authsignal/sdk-php/) — Official PHP SDK for the Authsignal Server API.
- [Authsignal Go SDK](https://apis.io/apis/authsignal/sdk-go/) — Official Go SDK for the Authsignal Server API.
- [Authsignal Browser SDK](https://apis.io/apis/authsignal/sdk-browser/) — JavaScript / TypeScript browser SDK wrapping the Client API and WebAuthn / passkey ceremonies for web applications.
- [Authsignal iOS SDK](https://apis.io/apis/authsignal/sdk-ios/) — Native iOS (Swift) SDK for passkeys, push, and OTP challenges in iOS applications.
- [Authsignal Android SDK](https://apis.io/apis/authsignal/sdk-android/) — Native Android (Kotlin) SDK for passkeys, push, and OTP challenges in Android applications.
- [Authsignal React Native SDK](https://apis.io/apis/authsignal/sdk-react-native/) — React Native wrapper around the iOS and Android SDKs.
- [Authsignal Flutter SDK](https://apis.io/apis/authsignal/sdk-flutter/) — Flutter (Dart) SDK wrapping the iOS and Android native SDKs.
- [Authsignal Actions API](https://apis.io/apis/authsignal/authsignal-actions-api/) — The Actions API from Authsignal — 3 operation(s) for actions.
- [Authsignal Authenticators API](https://apis.io/apis/authsignal/authsignal-authenticators-api/) — The Authenticators API from Authsignal — 4 operation(s) for authenticators.
- [Authsignal Challenges API](https://apis.io/apis/authsignal/authsignal-challenges-api/) — The Challenges API from Authsignal — 5 operation(s) for challenges.
- [Authsignal Devices API](https://apis.io/apis/authsignal/authsignal-devices-api/) — The Devices API from Authsignal — 3 operation(s) for devices.
- [Authsignal Sessions API](https://apis.io/apis/authsignal/authsignal-sessions-api/) — The Sessions API from Authsignal — 5 operation(s) for sessions.
- [Authsignal Users API](https://apis.io/apis/authsignal/authsignal-users-api/) — The Users API from Authsignal — 2 operation(s) for users.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Authsignal Agentic Access](https://apis.io/agentic-access/authsignal/authsignal-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Authsignal Server API](https://apis.io/collections/authsignal/open-authsignal/)
- [Authsignal Server Actions API](https://apis.io/collections/authsignal/open-authsignal-actions-api/)
- [Authsignal Server Actions Authenticators API](https://apis.io/collections/authsignal/open-authsignal-authenticators-api/)
- [Authsignal Server Actions Challenges API](https://apis.io/collections/authsignal/open-authsignal-challenges-api/)
- [Authsignal Server Actions Devices API](https://apis.io/collections/authsignal/open-authsignal-devices-api/)
- [Authsignal Server Actions Sessions API](https://apis.io/collections/authsignal/open-authsignal-sessions-api/)
- [Authsignal Server Actions Users API](https://apis.io/collections/authsignal/open-authsignal-users-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Authsignal Authentication](https://apis.io/security/authsignal/authsignal-authentication/)
- [Authsignal Domain Security](https://apis.io/security/authsignal/authsignal-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Authsignal Plans Pricing](https://apis.io/plans/authsignal/authsignal-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Authsignal Rate Limits](https://apis.io/rate-limits/authsignal/authsignal-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Authsignal Finops](https://apis.io/finops/authsignal/authsignal-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.authsignal.com/)
- [Documentation](https://docs.authsignal.com/)
- [Pricing](https://www.authsignal.com/pricing)
- [Blog](https://www.authsignal.com/blog)

## API Evangelist rating

**Kin Score 28.1** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 46.9 |
| Contract governance | 0.0 |
| Operational transparency | 26.3 |
| Developer ergonomics | 23.8 |
| Access clarity | 15.8 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
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

**Regulatory alignment 11.3** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/authsignal/](https://apis.io/providers/authsignal/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Authsignal: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/authsignal/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
