# Suki AI (suki)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Suki is a Redwood City, California healthcare AI company building ambient clinical intelligence for clinicians. Founded in 2017 by Punit Soni (CEO, former Google and Flipkart) and Karthik Rajan (former Salesforce), Suki has raised $168M+ across Series A-D from Venrock, March Capital, First Round Capital, MedStar Health, and others. The company's flagship product is Suki Assistant, an AI-powered voice-enabled scribe and documentation assistant that listens to doctor-patient conversations and generates specialty-specific clinical notes, patient instructions, orders, and codes — claimed to cut documentation time by 72% across 100+ specialties. Beyond the end-user assistant, Suki ships Suki Platform (also called Suki for Partners), a developer platform whose Suki Speech Service exposes ambient documentation, dictation, and form-filling capabilities as REST APIs, WebSocket audio-streaming endpoints, webhooks, and SDKs (Web, Headless Web, Mobile iOS, Mobile Android beta, Dictation iframe) so healthcare technology companies can embed Suki's voice AI into their own EHR, telehealth, RCM, or vet-tech applications. Suki has bidirectional ambient integrations with the four leading EHRs — Epic, Oracle Health (Cerner), athenahealth, and MEDITECH — plus partnerships with Amwell, Zoom, HealthEdge, WellSky, MEDENT, and Bond Vet, and is deployed at 400+ health systems and partners with a 70%+ clinician adoption rate.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Ambient Clinical Intelligence
- Medical Scribe
- Clinical Documentation
- Voice AI
- Speech Recognition
- Healthcare
- EHR Integration
- Epic
- Oracle Health
- athenahealth
- MEDITECH
- Dictation
- Form Filling
- Note Generation
- Generative AI
- HIPAA
- SOC2
- Healthcare Technology

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Suki Ambient API

REST + WebSocket API that powers ambient clinical documentation. Partners create an ambient session, seed it with patient/encounter context, stream microphone audio over WebSocket, end the session, then poll for and retrieve the generated clinical note, transcript, structured data, and recording. Supports 100+ medical specialties, 80+ spoken languages with English note output, speaker diarization, problem-based charting (PBC), and LOINC-coded note sections.

- **Human URL:** [https://developer.suki.ai/api-reference/overview](https://developer.suki.ai/api-reference/overview)
- **Base URL:** `https://sdp.suki-stage.com/api/v1/`

#### Tags

- Ambient
- Clinical Documentation
- Note Generation
- Speech Recognition
- WebSocket

#### Properties

- [Documentation](https://developer.suki.ai/api-reference/overview)
- [Documentation](https://developer.suki.ai/documentation/overview)
- [OpenAPI](openapi/suki-ambient-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/suki-ambient-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/suki-ambient-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/suki-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/suki-ambient-session-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/suki-clinical-note-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [SDK](https://developer.suki.ai/web-sdk/overview)
- [SDK](https://developer.suki.ai/headless-web-sdk/introduction)
- [SDK](https://developer.suki.ai/mobile-sdk/overview)
- [Webhooks](https://developer.suki.ai/api-reference/overview)

### Suki Dictation API

REST + WebSocket API for real-time clinical dictation. Partners open a dictation session, stream audio to a WebSocket, and receive transcribed clinical text. Designed for both in-field dictation (into a single EHR field) and scratchpad mode for free-form capture. Also exposed through the Suki Dictation SDK as a hosted iframe for fast web integration.

- **Human URL:** [https://developer.suki.ai/api-reference/ambient-dictation](https://developer.suki.ai/api-reference/ambient-dictation)
- **Base URL:** `https://sdp.suki-stage.com/api/v1/`

#### Tags

- Dictation
- Speech Recognition
- WebSocket
- Clinical Voice

#### Properties

- [Documentation](https://developer.suki.ai/api-reference/ambient-dictation)
- [OpenAPI](openapi/suki-dictation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/suki-dictation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/suki-dictation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/suki-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [SDK](https://developer.suki.ai/dictation-sdk/introduction)

### Suki Form Filling API

REST + WebSocket API that turns clinician voice input into structured form data. Partners create a form-filling session, attach a template, stream audio, then retrieve typed structured output that can be mapped into their own intake, screening, or assessment forms. Includes Suki-hosted form templates accessed via a templates listing endpoint.

- **Human URL:** [https://developer.suki.ai/form-filling-api-reference/overview](https://developer.suki.ai/form-filling-api-reference/overview)
- **Base URL:** `https://sdp.suki-stage.com/api/v1/`

#### Tags

- Form Filling
- Structured Data
- Voice Capture
- WebSocket

#### Properties

- [Documentation](https://developer.suki.ai/form-filling-api-reference/overview)
- [OpenAPI](openapi/suki-form-filling-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/suki-form-filling-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/suki-form-filling-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/suki-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/suki-form-template-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Webhooks](https://developer.suki.ai/form-filling-api-reference/overview)

### Suki Auth API

Authentication and token-issuance endpoints used by partners and partner-managed providers to obtain access tokens for the Suki Speech Service. Issues JWTs, exposes JWKS for verification, and registers provider accounts. Every call to Ambient, Dictation, and Form Filling APIs carries the partner token in the `sdp_suki_token` header.

- **Human URL:** [https://developer.suki.ai/api-reference/authentication](https://developer.suki.ai/api-reference/authentication)
- **Base URL:** `https://sdp.suki-stage.com/api/v1/`

#### Tags

- Authentication
- Tokens
- JWT
- JWKS

#### Properties

- [Documentation](https://developer.suki.ai/api-reference/authentication)
- [OpenAPI](openapi/suki-auth-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/suki-auth-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/suki-auth-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Suki Info API

Reference/lookup endpoints that expose Suki-curated clinical metadata used to drive note generation, ordering, and form filling. Covers supported specialties, diagnoses, encounter and visit types, LOINC note sections, provider roles, medication orders, order coding systems, dosage units, and form templates.

- **Human URL:** [https://developer.suki.ai/api-reference/information](https://developer.suki.ai/api-reference/information)
- **Base URL:** `https://sdp.suki-stage.com/api/v1/`

#### Tags

- Reference Data
- Metadata
- Specialties
- LOINC
- Medication Orders

#### Properties

- [Documentation](https://developer.suki.ai/api-reference/information)
- [OpenAPI](openapi/suki-info-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/suki-info-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/suki-info-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.suki.ai)
- [About](https://www.suki.ai/about/)
- [Clinicians](https://www.suki.ai/clinicians/)
- [Technology](https://www.suki.ai/technology/)
- [Platform](https://www.suki.ai/platform/)
- [Partners](https://www.suki.ai/partners/)
- [E H R Integrations](https://www.suki.ai/ehr-integrations/)
- [Epic](https://www.suki.ai/epic/)
- [athenahealth](https://www.suki.ai/athena/)
- [Developer Portal](https://developer.suki.ai/)
- [Documentation](https://developer.suki.ai/documentation/overview)
- [API Reference](https://developer.suki.ai/api-reference/overview)
- [Release Notes](https://developer.suki.ai/updates/release-notes)
- [L L Ms Txt](https://developer.suki.ai/llms.txt)
- [Help Center](https://help.suki.ai)
- [Trust Portal](https://trust.suki.ai)
- [Blog](https://www.suki.ai/blog/)
- [Newsroom](https://www.suki.ai/news/)
- [Press Releases](https://www.suki.ai/press-media/)
- [Careers](https://www.suki.ai/careers/)
- [Contact](https://www.suki.ai/contact-us/)
- [Download](https://www.suki.ai/download/)
- [App Store](https://apps.apple.com/us/app/suki/id1425102117)
- [LinkedIn](https://www.linkedin.com/company/sukihq/)
- [Plans](plans/suki-plans-pricing.yml)
- [Rate Limits](rate-limits/suki-rate-limits.yml)
- [Fin Ops](finops/suki-finops.yml)
- [JSON-LD](json-ld/suki-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/suki-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
