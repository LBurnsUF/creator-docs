---
title: Ordered Data Stores / V1 / Universes
type: cloud-api
tags: [Data and memory stores]
---

# Ordered Data Stores / V1 / Universes

Cloud API resource group with 6 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries` | Returns a list of entries from an ordered data store. [BETA] |
| `POST` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries` | Creates a new entry with the content value provided. [BETA] |
| `DELETE` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}` | Deletes the specified entry. Unlike standard data stores, which mark entries for deletion, ordered d [BETA] |
| `GET` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}` | Gets and returns the specified entry. [BETA] |
| `PATCH` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}` | Updates an entry value and returns the updated entry. [BETA] |
| `POST` | `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}:increment` | Increments the value of the key by the provided amount and returns the updated entry.  Known issue:  [BETA] |

### `GET` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries`

**Operation:** `OrderedDataStores_ListEntries`

**Stability:** BETA

Returns a list of entries from an ordered data store.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the target ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `max_page_size` (query, integer) - The maximum number of entries to return. The service may return fewer than this value. The default value is `10`. The maximum value is `100`, and any 
- `page_token` (query, string) - A page token received from a previous `List` call. Provide this to retrieve the subsequent page. When paginating, all other parameters provided to `Li
- `order_by` (query, string) - The enumeration direction. The order by default is ascending. Input a `desc` suffix for descending.
- `filter` (query, string) - The range of qualifying values of entries to return. See [Filters](/cloud/guides/data-stores/request-handling.md#filters).

**Responses:**

- `200` - OK
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: studio access to APIs is not allowed, incorrect API key or scope.
- `429` - Too Many Requests.

### `POST` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries`

**Operation:** `OrderedDataStores_CreateEntry`

**Stability:** BETA

Creates a new entry with the content value provided.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `id` (query, string (required)) - The name of the entry.

**Responses:**

- `200` - OK
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: studio access to APIs is not allowed, incorrect API key or scope.
- `404` - Not found.
- `429` - Too Many Requests.

### `DELETE` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}`

**Operation:** `OrderedDataStores_DeleteEntry`

**Stability:** BETA

Deletes the specified entry. Unlike standard data stores, which mark entries for deletion, ordered data store entries are deleted immediately.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `entry` (path, string (required)) - The entry ID.

**Responses:**

- `200` - Success: the entry was successfully deleted or didn't exist.
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: Studio access to APIs is not allowed, incorrect API key or scope.
- `404` - Not found.
- `429` - Too Many Requests.

### `GET` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}`

**Operation:** `OrderedDataStores_GetEntry`

**Stability:** BETA

Gets and returns the specified entry.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `entry` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: studio access to APIs is not allowed, incorrect API key or scope.
- `404` - Not found.
- `429` - Too Many Requests.

### `PATCH` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}`

**Operation:** `OrderedDataStores_UpdateEntry`

**Stability:** BETA

Updates an entry value and returns the updated entry.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `entry` (path, string (required)) - The entry ID.
- `allow_missing` (query, boolean) - The flag to allow the creation of an entry if the entry doesn't exist. See [Allow missing flags](/cloud/guides/data-stores/request-handling.md.md#allo

**Responses:**

- `200` - OK
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: studio access to APIs is not allowed, incorrect API key or scope.
- `404` - Not found.
- `409` - Aborted.
- `429` - Too Many Requests.

### `POST` `/ordered-data-stores/v1/universes/{universeId}/orderedDataStores/{orderedDataStore}/scopes/{scope}/entries/{entry}:increment`

**Operation:** `OrderedDataStores_IncrementEntry`

**Stability:** BETA

Increments the value of the key by the provided amount and returns the updated entry.

Known issue: Entry values can increment past the valid range and this may persist in the backend. Returned values will clamp to the valid range.

**Parameters:**

- `universeId` (path, string (required)) - The identifier of the experience with ordered data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `orderedDataStore` (path, string (required)) - The name of the ordered data store.
- `scope` (path, string (required)) - The name of the data store scope. See [Scopes](/cloud/guides/data-stores/request-handling.md#scopes).
- `entry` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK
- `400` - Bad Request: invalid orderedDataStore, scope or entry name or encoding.
- `403` - Forbidden: studio access to APIs is not allowed, incorrect API key or scope.
- `404` - Not found.
- `429` - Too Many Requests.
