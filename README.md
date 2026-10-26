# Pieces (pieces)

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

Pieces is an on-device AI developer assistant and long-term memory tool. Pieces OS runs locally on the developer's machine and exposes a documented local REST API at http://localhost:1000 covering saved snippets (assets), the Pieces Copilot (QGPT) question/stream endpoints, local and cloud models, formats, applications, conversations, and workspace context. The same on-device API powers official OpenAPI-generated SDKs for Python, TypeScript, Dart, Kotlin, and C#.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/apis.yml)

## Tags

- AI
- Developer Tools
- On-Device
- Local API
- Long-Term Memory

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Pieces Assets API

Create, read, update, delete, search, and stream saved snippets (assets) held in the local Pieces OS database. Served on-device over the localhost REST transport - no data leaves the machine unless the user opts into cloud sync.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Assets
- Snippets
- On-Device

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

### Pieces Copilot (QGPT) API

The Pieces Copilot generative engine (QGPT). Ask questions grounded in relevant local snippets via POST /qgpt/question, score relevance, reprompt, and open a WebSocket at /qgpt/stream for streamed, multi-turn conversational answers. Runs against local or cloud LLMs from the on-device Pieces OS process.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Copilot
- QGPT
- Conversations

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/pieces-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

### Pieces Conversations API

Manage Copilot conversations and their messages locally - create, list, rename, search, summarize, and delete conversations, and create/update/search the messages within them. Stored in the on-device Pieces OS database.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Conversations
- Messages
- Copilot

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

### Pieces Models API

Enumerate and manage the LLMs available to Pieces OS - list models, download/load/unload local models (e.g. Llama, Mistral via on-device runtime), track download progress, and delete model caches. Local models run fully on-device; cloud models are routed through the same local API surface.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Models
- LLM
- On-Device

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

### Pieces Formats API

Read, update, reclassify, and analyze the underlying formats (code or text fragment representations) that back each asset. Served on-device by Pieces OS over the localhost transport.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Formats
- Classification
- Fragments

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

### Pieces Applications & Workspace API

Register applications, open/close application sessions, read the well-known health and version of the local Pieces OS instance, and manage user and OS-level context (device information, settings, sign-in). The control plane for the on-device Pieces OS process.

- **Human URL:** [https://docs.pieces.app/products/core-dependencies/pieces-os](https://docs.pieces.app/products/core-dependencies/pieces-os)
- **Base URL:** `http://localhost:1000`

#### Tags

- Applications
- Workspace
- OS

#### Properties

- [Documentation](https://docs.pieces.app/products/core-dependencies/pieces-os)
- [API Reference](https://github.com/pieces-app/pieces-os-client-openapi-spec)
- [OpenAPI](openapi/pieces-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pieces.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pieces.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/pieces-app)

## Common Properties

- [GitHub Organization](https://github.com/pieces-app)
- [LinkedIn](https://www.linkedin.com/company/getpieces)
- [Website](https://pieces.app)
- [Documentation](https://docs.pieces.app)
- [Plans](plans/pieces-plans-pricing.yml)
- [Rate Limits](rate-limits/pieces-rate-limits.yml)
- [Fin Ops](finops/pieces-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
