# Huly (huly)

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
