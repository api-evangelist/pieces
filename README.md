# Pieces (pieces)

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
