---
title: Creator Configs Public Api / V1 / Configs
type: cloud-api
tags: [Configs]
---

# Creator Configs Public Api / V1 / Configs

Cloud API resource group with 9 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}` | Gets published config values without metadata. [BETA] |
| `DELETE` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft` | Resets (deletes) the current draft. [BETA] |
| `GET` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft` | Gets the current draft. [BETA] |
| `PATCH` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft` | Partially updates the draft. [BETA] |
| `PUT` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft:overwrite` | Overwrites the entire draft with the request payload. [BETA] |
| `GET` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/full` | Gets full config with metadata. [BETA] |
| `POST` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/publish` | Publishes draft changes. [BETA] |
| `GET` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/revisions` | Lists revision history. [BETA] |
| `POST` | `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/revisions/{revisionId}/restore` | Stages a revert to a previous revision. [BETA] |

### `GET` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}`

**Operation:** `CreatorConfigsPublicApi_GetConfigRepositoryValues`

**Stability:** BETA

Returns the latest published config values without metadata and decorators.
This response can be used as a direct copy-and-paste to the draft update endpoints.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `DELETE` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft`

**Operation:** `CreatorConfigsPublicApi_DeleteDraft`

**Stability:** BETA

Resets the current draft area. If draftHash is provided, this call will fail if the hash doesn't match.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `GET` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft`

**Operation:** `CreatorConfigsPublicApi_GetConfigRepositoryDraft`

**Stability:** BETA

Returns the current draft changes for the configuration repository.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `PATCH` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft`

**Operation:** `CreatorConfigsPublicApi_UpdateDraft`

**Stability:** BETA

Updates the draft treating the payload as a partial changeset.
If draftHash is provided, this call will fail if the hash doesn't match.
A key not included will not be changed. To indicate deletion, set key to null.
To discard a change, set key to its currently published value.
When `conditionalRules` is omitted or empty (`{}`), the CMS update omits the conditional-rules field so existing published rules remain at publish time;
send a non-empty `conditionalRules` object to merge rule changes.
Entry count and per-value size limits are enforced here via CreatorConfigsPublicApi.Utils.DraftValidationHelper; further schema validation is performed by Config Management.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `PUT` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/draft:overwrite`

**Operation:** `CreatorConfigsPublicApi_OverwriteDraft`

**Stability:** BETA

Full overwrite of current draft. The payload is the expected final state after publish (not a merge with the draft or published config from the client’s perspective).
The service aligns that intent with CMS validation by emitting explicit deletions for published keys and conditional branches omitted from the body.
If a key is not included, it is interpreted as removed.
When `conditionalRules` is included, `conditionalRules.rules` is authoritative for rule definitions:
any conditional rule that exists on the latest published configuration but is omitted from `rules` is removed (same as sending an empty RPN rule).
When `conditionalRules` is omitted, all published conditional rules are removed; entries must not use conditional branches or `.RBX.conditional.*` keys unless you send `conditionalRules`.
If draftHash is provided, this call will fail if the hash doesn't match.
Entry count and per-value size limits are enforced here via CreatorConfigsPublicApi.Utils.DraftValidationHelper;...

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `GET` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/full`

**Operation:** `CreatorConfigsPublicApi_GetConfigRepositoryFull`

**Stability:** BETA

Returns the full config including metadata (version, descriptions, last modified/accessed times).

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `POST` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/publish`

**Operation:** `CreatorConfigsPublicApi_PublishDraft`

**Stability:** BETA

Applies the current draft to the published config. Requires a draft hash and optional message and deployment strategy.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `GET` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/revisions`

**Operation:** `CreatorConfigsPublicApi_ListRevisions`

**Stability:** BETA

Returns the list of previous revisions to the repository. Supports optional start/end time and pagination.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig
- `startTime` (query, string) - Optional start time for filtering revisions.
- `endTime` (query, string) - Optional end time for filtering revisions.
- `MaxPageSize` (query, string) - Maximum page size.
- `Skip` (query, string) - Number of items to skip.
- `SearchKey` (query, string) - Search key to filter by.
- `SortOrder` (query, string) - Sort order (e.g., "SORT_ORDER_DESCENDING", "SORT_ORDER_ASCENDING").
- `SortKey` (query, string) - Sort key (e.g., "SORT_KEY_LAST_MODIFIED_TIME").

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found

### `POST` `/creator-configs-public-api/v1/configs/universes/{universeId}/repositories/{repository}/revisions/{revisionId}/restore`

**Operation:** `CreatorConfigsPublicApi_RestoreRevision`

**Stability:** BETA

Attempts to restore configs to the provided revision. This will clear the staging and stage a revert commit.
You must call publish for the revert to take effect.

**Parameters:**

- `universeId` (path, string (required)) - 
- `repository` (path (required)) -   InExperienceConfig  RecommendationServicesConfig  DataStoresConfig  ExtendedServicesConfig  LeaderboardsConfig  ExperienceUserConfig  JourneysConfig
- `revisionId` (path, string (required)) - 

**Responses:**

- `200` - OK
- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found
