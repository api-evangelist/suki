# Suki AI

Suki is a Redwood City, California healthcare AI company (founded 2017 by Punit Soni and Karthik Rajan; $168M+ raised through Series D) that builds ambient clinical intelligence for clinicians. Suki Assistant listens to doctor-patient conversations and generates specialty-specific clinical notes, patient instructions, orders, and codes — cutting documentation time by an industry-reported 72% across 100+ medical specialties. Beyond the end-user app, the Suki Platform (Suki for Partners) exposes the Suki Speech Service to healthcare technology partners as REST APIs, WebSocket audio streaming, webhooks, and Web / Mobile / Dictation SDKs.

Suki has bidirectional ambient integrations with the four leading EHRs — Epic, Oracle Health (Cerner), athenahealth, and MEDITECH — and partners with Amwell, Zoom, HealthEdge, WellSky, MEDENT, and Bond Vet. The platform is HIPAA compliant and SOC 2 Type 2 certified, deployed at 400+ health systems with a reported 70%+ clinician adoption rate.

## APIs

- **Suki Ambient API** — Ambient session lifecycle (create, seed context, end, status) plus content retrieval (note, transcript, recording, structured data), preferences, and feedback. Pairs with a WebSocket audio stream and webhooks. [`openapi/suki-ambient-api-openapi.yml`](openapi/suki-ambient-api-openapi.yml)
- **Suki Dictation API** — Real-time clinical dictation with in-field and scratchpad modes. [`openapi/suki-dictation-api-openapi.yml`](openapi/suki-dictation-api-openapi.yml)
- **Suki Form Filling API** — Voice-driven population of structured medical forms against Suki-hosted templates. [`openapi/suki-form-filling-api-openapi.yml`](openapi/suki-form-filling-api-openapi.yml)
- **Suki Auth API** — Partner login, provider registration, and JWKS for verifying `sdp_suki_token` JWTs. [`openapi/suki-auth-api-openapi.yml`](openapi/suki-auth-api-openapi.yml)
- **Suki Info API** — Read-only catalogs of specialties, diagnoses, encounter / visit types, LOINC sections, medication orders, coding systems, and dosage units. [`openapi/suki-info-api-openapi.yml`](openapi/suki-info-api-openapi.yml)

## Developer Surface

- Developer Portal: https://developer.suki.ai/
- Documentation Overview: https://developer.suki.ai/documentation/overview
- API Reference: https://developer.suki.ai/api-reference/overview
- Form Filling Reference: https://developer.suki.ai/form-filling-api-reference/overview
- Release Notes: https://developer.suki.ai/updates/release-notes
- Base URL: `https://sdp.suki-stage.com/api/v1/`
- Auth header: `sdp_suki_token: <jwt>`
- SDKs: `@suki-sdk/react` (Web), `@suki-sdk/platform-react` (Headless Web, beta), `@suki-sdk/dictation-react` (Dictation, beta), `SukiAmbientCore.framework` (iOS); Android coming soon.

## Naftiko Capabilities

- [`capabilities/ambient-sessions.yaml`](capabilities/ambient-sessions.yaml)
- [`capabilities/ambient-content.yaml`](capabilities/ambient-content.yaml)
- [`capabilities/dictation-sessions.yaml`](capabilities/dictation-sessions.yaml)
- [`capabilities/form-filling-sessions.yaml`](capabilities/form-filling-sessions.yaml)
- [`capabilities/auth-tokens.yaml`](capabilities/auth-tokens.yaml)
- [`capabilities/info-reference.yaml`](capabilities/info-reference.yaml)

## Other Artifacts

- JSON Schema: [`json-schema/`](json-schema/) — ambient session, clinical note, form template
- JSON-LD context: [`json-ld/suki-context.jsonld`](json-ld/suki-context.jsonld)
- Vocabulary: [`vocabulary/suki-vocabulary.yml`](vocabulary/suki-vocabulary.yml)
- Plans / pricing: [`plans/suki-plans-pricing.yml`](plans/suki-plans-pricing.yml)
- Rate limits: [`rate-limits/suki-rate-limits.yml`](rate-limits/suki-rate-limits.yml)
- FinOps: [`finops/suki-finops.yml`](finops/suki-finops.yml)
- Examples: [`examples/`](examples/)

## Compliance

- HIPAA
- SOC 2 Type 2
- Trust Portal: https://trust.suki.ai

## Links

- Website: https://www.suki.ai
- About: https://www.suki.ai/about/
- Platform: https://www.suki.ai/platform/
- Partners: https://www.suki.ai/partners/
- EHR Integrations: https://www.suki.ai/ehr-integrations/
- Blog: https://www.suki.ai/blog/
- Newsroom: https://www.suki.ai/news/
- Careers: https://www.suki.ai/careers/
- Contact: https://www.suki.ai/contact-us/
- LinkedIn: https://www.linkedin.com/company/sukihq/
- iOS App: https://apps.apple.com/us/app/suki/id1425102117
