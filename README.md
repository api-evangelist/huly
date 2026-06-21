# Huly (huly)

Huly is an open-source, all-in-one project management and team collaboration platform (an alternative to Linear, Jira, Slack, and Notion) built around modules like Tracker and Documents. Programmatic access is delivered primarily as a Node.js SDK (@hcengineering/api-client) that connects to the platform transactor over WebSocket or REST, rather than a broad public HTTP API. Huly is available as free, self-hostable open source (github.com/hcengineering) and as managed Huly Cloud.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/apis.yml)

## Tags

- Project Management
- Collaboration
- Open Source
- Productivity
- SDK

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Huly Platform SDK

The @hcengineering/api-client Node.js package provides typed programmatic access to the Huly Platform. It exposes a WebSocket client (connect) holding a persistent transactor connection and a REST client (connectRest), both authenticated by email/password or token, with document operations such as findOne, findAll, createDoc, updateDoc, and removeDoc. There is no broadly documented public HTTP REST API with stable URL paths; access is intended through this SDK.

- **Human URL:** [https://github.com/hcengineering/huly.core/blob/main/packages/api-client/README.md](https://github.com/hcengineering/huly.core/blob/main/packages/api-client/README.md)
- **Base URL:** `https://github.com/hcengineering/huly.core`

#### Tags

- SDK
- Platform
- WebSocket
- REST

#### Properties

- [Documentation](https://github.com/hcengineering/huly.core/blob/main/packages/api-client/README.md)
- [API Reference](https://github.com/hcengineering/huly-examples/tree/main/platform-api)
- [OpenAPI](openapi/huly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/huly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/huly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Huly Cloud

Managed, hosted Huly offered as Huly Cloud with usage-tiered workspaces (Common, Rare, Epic, Legendary, and custom Enterprise plans). Cloud workspaces run the same platform and are reachable programmatically through the Huly Platform SDK against the hosted account and transactor services.

- **Human URL:** [https://huly.io/](https://huly.io/)
- **Base URL:** `https://huly.io/`

#### Tags

- Cloud
- SaaS
- Hosting

#### Properties

- [Documentation](https://docs.huly.io/)
- [API Reference](https://docs.huly.io/getting-started/api-tools/)
- [OpenAPI](openapi/huly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/huly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/huly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Huly Tracker

Tracker is Huly's project and issue management module (subtasks, milestones, templates, custom workflows) with optional two-way GitHub Issues/Projects sync. Issues, projects, and related objects are accessed programmatically as platform documents through the Huly Platform SDK rather than via a dedicated public REST API.

- **Human URL:** [https://huly.io/](https://huly.io/)
- **Base URL:** `https://github.com/hcengineering/huly.core`

#### Tags

- Issue Tracking
- Project Management
- Agile

#### Properties

- [Documentation](https://docs.huly.io/)
- [API Reference](https://github.com/hcengineering/huly-examples/tree/main/platform-api)
- [OpenAPI](openapi/huly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/huly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/huly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Huly Documents

Documents is Huly's collaborative knowledge-management module for rich-text documents with code blocks and real-time editing. Document content is modeled as platform markup and accessed through the Huly Platform SDK's document and collaborative markup operations rather than a standalone public REST API.

- **Human URL:** [https://huly.io/](https://huly.io/)
- **Base URL:** `https://github.com/hcengineering/huly.core`

#### Tags

- Documents
- Knowledge Management
- Collaboration

#### Properties

- [Documentation](https://docs.huly.io/)
- [API Reference](https://github.com/hcengineering/huly-examples/tree/main/platform-api)
- [OpenAPI](openapi/huly-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/huly.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/huly.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/hcengineering)
- [LinkedIn](https://www.linkedin.com/company/hardcoreeng)
- [Website](https://huly.io/)
- [Documentation](https://docs.huly.io/)
- [Plans](plans/huly-plans-pricing.yml)
- [Rate Limits](rate-limits/huly-rate-limits.yml)
- [Fin Ops](finops/huly-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
