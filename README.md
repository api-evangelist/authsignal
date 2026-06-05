# Authsignal (authsignal)

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
