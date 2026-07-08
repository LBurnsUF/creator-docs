---
title: Datastores / V1 / Universes
type: cloud-api
tags: [Data and memory stores]
---

# Datastores / V1 / Universes

Cloud API resource group with 8 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/datastores/v1/universes/{universeId}/standard-datastores` | List data stores in an experience [BETA] |
| `GET` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries` | List entries [BETA] |
| `DELETE` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry` | Delete entry. [BETA] |
| `GET` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry` | Get entry. [BETA] |
| `POST` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry` | Set entry. [BETA] |
| `POST` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/increment` | Increment entry [BETA] |
| `GET` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/versions` | List entry versions [BETA] |
| `GET` | `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/versions/version` | Get entry version. [BETA] |

### `GET` `/datastores/v1/universes/{universeId}/standard-datastores`

**Operation:** `Datastores_ListDatastoresAsync`

**Stability:** BETA

Returns a list of an experience's data stores.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `cursor` (query, string) - Provide to request the next set of data.
- `limit` (query, integer) - The maximum number of items to return. Each call only reads one partition, so it can return fewer than the given value when running out of objectives 
- `prefix` (query, string) - Provide to return only data stores with this prefix. 

**Responses:**

- `200` - 

### `GET` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries`

**Operation:** `Entries_ListKeysAsync`

**Stability:** BETA

Returns a list of entry keys within a data store.

 Entries marked deleted with a tombstone version are still included in the response if they have yet to be permanently deleted.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).
- `allScopes` (query, boolean) - Set to true to return keys from all scopes.
- `prefix` (query, string) - Provide to return only keys with this prefix.
- `cursor` (query, string) - Provide to request the next set of data.
- `limit` (query, integer) - The maximum number of items to return. Each call only reads one partition, so it can return fewer than the given value when running out of objectives 

**Responses:**

- `200` - 

### `DELETE` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry`

**Operation:** `Entries_DeleteEntryAsync`

**Stability:** BETA

Marks the entry as deleted by creating a tombstone version. Entries are deleted permanently after 30 days.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).

**Responses:**

- `204` - The entry is deleted.

### `GET` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry`

**Operation:** `Entries_GetEntryAsync`

**Stability:** BETA

Returns the value and metadata associated with an entry.

Entries marked deleted with a tombstone version will return 404 Not Found.

Metadata can be found in the response headers like the following:
```text
content-md5: zuYxEhwuySMv0i8CitXImw==
roblox-entry-version: 08D9E6A3F2188CFF.0000000001.08D9E6A3F2188CFF.01
roblox-entry-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-version-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-attributes: { "myAttribute": "myValue" }
roblox-entry-userids: [1, 2, 3]
```

| Header | Description |
|---|---| 
| `content-md5` | The base64-encoded MD5 checksum of the content. See [Content-MD5](/cloud/guides/data-stores/request-handling.md#content-md5). |
| `roblox-entry-version` | The version of the returned entry. |
| `roblox-entry-created-time` | The time at which the entry was created. |
| `roblox-entry-version-created-time` | The time at which this particular version was created. |
| `roblox-entry-attributes` | Attributes tagg...

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).

**Responses:**

- `200` - Successfully retrieved the entry.
- `204` - The key is marked as deleted.

### `POST` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry`

**Operation:** `Entries_SetEntryAsync`

**Stability:** BETA

Sets the value, metadata and user IDs associated with an entry.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `matchVersion` (query, string) - Provide to update only if the current version matches this.
- `exclusiveCreate` (query, boolean) - Create the entry only if it does not exist.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).
- `roblox-entry-attributes` (header, string) - Attributes to be associated with new version of the entry. Serialized by JSON map objects. If not provided, existing attributes are cleared.
- `roblox-entry-userids` (header, string) - Comma-separated list of Roblox user IDs tagged with the entry. If not provided, existing user IDs are cleared.
- `content-md5` (header, string) - The base64-encoded MD5 checksum of the content. See [Content-MD5](/cloud/guides/data-stores/request-handling.md#content-md5).

**Responses:**

- `200` - 

### `POST` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/increment`

**Operation:** `Entries_IncrementEntryAsync`

**Stability:** BETA

Increments the value for an entry by a given amount, or create a new entry with that amount. Returns the entry and metadata.

Metadata can be found in the response headers like the following:
```text
content-md5: zuYxEhwuySMv0i8CitXImw==
roblox-entry-version: 08D9E6A3F2188CFF.0000000001.08D9E6A3F2188CFF.01
roblox-entry-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-version-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-attributes: { "myAttribute": "myValue" }
roblox-entry-userids: [1, 2, 3]
```

| Header | Description |
|---|---| 
| `content-md5` | The base64-encoded MD5 checksum of the content. See [Content-MD5](/cloud/guides/data-stores/request-handling.md#content-md5). |
| `roblox-entry-version` | The version of the returned entry. |
| `roblox-entry-created-time` | The time at which the entry was created. |
| `roblox-entry-version-created-time` | The time at which this particular version was created. |
| `roblox-entry-attributes` | Attributes tagged with ...

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `incrementBy` (query, integer) - The amount by which the entry should be incremented, or the starting value if it doesn't exist.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).
- `roblox-entry-attributes` (header, string) - Attributes to be associated with new version of the entry. Serialized by JSON map objects. If not provided, existing attributes are cleared.
- `roblox-entry-userids` (header, string) - A comma-separated list of Roblox user IDs that the entry is tagged with. If not provided, existing user IDs are cleared.

**Responses:**

- `200` - Returns the latest version of the entry after it has been incremented.
- `204` - The key is marked as deleted.

### `GET` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/versions`

**Operation:** `Entries_ListEntryVersionsAsync`

**Stability:** BETA

Returns a list of versions for an entry.

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).
- `cursor` (query, string) - Provide to request the next set of data.
- `startTime` (query, string) - Provide to not include versions earlier than this timestamp.
- `endTime` (query, string) - Provide to not include versions later than this timestamp.
- `sortOrder` (query, string) - Either `Ascending` (earlier versions first) or `Descending` (later versions first).
- `limit` (query, integer) - The maximum number of items to return. Each call only reads one partition, so it can return fewer than the given value when running out of objectives 

**Responses:**

- `200` - 
- `400` - Invalid request / Invalid file content.
- `403` - Publish not allowed on place.
- `404` - The experience or data store was not found.
- `429` - Too Many Requests.

### `GET` `/datastores/v1/universes/{universeId}/standard-datastores/datastore/entries/entry/versions/version`

**Operation:** `Entries_GetEntryVersionAsync`

**Stability:** BETA

Returns the value and metadata of a specific version of an entry.

Metadata can be found in the response headers like the following:
```text
content-md5: zuYxEhwuySMv0i8CitXImw==
roblox-entry-version: 08D9E6A3F2188CFF.0000000001.08D9E6A3F2188CFF.01
roblox-entry-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-version-created-time: 2022-02-02T23:30:06.5388799+00:00
roblox-entry-attributes: { "myAttribute": "myValue" }
roblox-entry-userids: [1, 2, 3]
```

| Header | Description |
|---|---| 
| `content-md5` | The base64-encoded MD5 checksum of the content. See [Content-MD5](/cloud/guides/data-stores/request-handling.md#content-md5). |
| `roblox-entry-version` | The version of the returned entry. |
| `roblox-entry-created-time` | The time at which the entry was created. |
| `roblox-entry-version-created-time` | The time at which this particular version was created. |
| `roblox-entry-attributes` | Attributes tagged with the entry. Serialized JSON map object. |
| `roblox-entry-us...

**Parameters:**

- `universeId` (path, integer (required)) - The identifier of the experience with data stores that you want to access. You can find your experience's universe ID on Creator Hub.
- `datastoreName` (query, string) - The name of the data store.
- `entryKey` (query, string) - The key identifying the entry.
- `versionId` (query, string) - The version to inspect.
- `scope` (query, string) - The value is `global` by default. See [Scopes](/cloud-services/data-stores/index.md#scopes).

**Responses:**

- `200` - Successfully retrieved the entry.
