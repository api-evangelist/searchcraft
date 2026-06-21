# Searchcraft (searchcraft)

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
