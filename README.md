# Searchcraft (searchcraft)

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

Searchcraft is a developer-first search engine and search-as-a-service platform. Its REST API lets teams create indexes, ingest and manage documents, run fuzzy/exact full-text search with facets and relevancy tuning, query across multiple indexes via federated search, and manage synonyms, stopwords, and usage measurement. It ships as a managed cloud service (Searchcraft Cloud) and a self-hosted engine (Searchcraft Core).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/apis.yml)

## Tags

- Search
- Search as a Service
- Full Text Search
- Indexing
- Developer Tools

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Searchcraft Index API

Create, read, replace, patch, and delete search indexes and their schemas, and retrieve per-index and cluster-wide document statistics. Requires an admin-tier authentication key.

- **Human URL:** [https://docs.searchcraft.io/api/index-management/](https://docs.searchcraft.io/api/index-management/)
- **Base URL:** `https://your-cluster.searchcraft.io`

#### Tags

- Indexes
- Schema
- Administration

#### Properties

- [Documentation](https://docs.searchcraft.io/api/index-management/)
- [OpenAPI](openapi/searchcraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searchcraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searchcraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searchcraft Documents / Ingest API

Add one or several documents to an index, retrieve a document by its internal id, and delete documents by id, by field term, by query, or all at once. Write transactions can be committed or rolled back. Requires an ingestion-tier authentication key.

- **Human URL:** [https://docs.searchcraft.io/api/document-management/](https://docs.searchcraft.io/api/document-management/)
- **Base URL:** `https://your-cluster.searchcraft.io`

#### Tags

- Documents
- Ingest
- Indexing

#### Properties

- [Documentation](https://docs.searchcraft.io/api/document-management/)
- [OpenAPI](openapi/searchcraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searchcraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searchcraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searchcraft Search API

Run full-text search against an index with fuzzy, exact, or dynamic query modes, Boolean should/must occurrence, facets, ordering, paging, and relevancy tuning. Requires a read-tier authentication key.

- **Human URL:** [https://docs.searchcraft.io/api/search/](https://docs.searchcraft.io/api/search/)
- **Base URL:** `https://your-cluster.searchcraft.io`

#### Tags

- Search
- Full Text Search
- Fuzzy Matching

#### Properties

- [Documentation](https://docs.searchcraft.io/api/search/)
- [OpenAPI](openapi/searchcraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searchcraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searchcraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searchcraft Federated Search API

Query across all indexes grouped into a federation in a single request, and manage federations (create, read, update, delete, stats). Searching requires a read-tier key; federation management requires admin.

- **Human URL:** [https://docs.searchcraft.io/api/search/](https://docs.searchcraft.io/api/search/)
- **Base URL:** `https://your-cluster.searchcraft.io`

#### Tags

- Federated Search
- Multi Index
- Search

#### Properties

- [Documentation](https://docs.searchcraft.io/api/search/)
- [OpenAPI](openapi/searchcraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searchcraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searchcraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Searchcraft Synonyms & Stopwords API

Manage per-index synonym sets (which apply to fuzzy queries only) and custom stopword lists used during relevancy tuning. Requires an ingestion-tier authentication key.

- **Human URL:** [https://docs.searchcraft.io/api/synonyms/](https://docs.searchcraft.io/api/synonyms/)
- **Base URL:** `https://your-cluster.searchcraft.io`

#### Tags

- Synonyms
- Stopwords
- Relevancy

#### Properties

- [Documentation](https://docs.searchcraft.io/api/synonyms/)
- [OpenAPI](openapi/searchcraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/searchcraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/searchcraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/searchcraft-inc)
- [LinkedIn](https://www.linkedin.com/company/searchcraft)
- [Website](https://www.searchcraft.io/)
- [Documentation](https://docs.searchcraft.io/)
- [Plans](plans/searchcraft-plans-pricing.yml)
- [Rate Limits](rate-limits/searchcraft-rate-limits.yml)
- [Fin Ops](finops/searchcraft-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
