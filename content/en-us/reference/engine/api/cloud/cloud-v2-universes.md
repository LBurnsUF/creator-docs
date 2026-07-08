---
title: Cloud / V2 / Universes
type: cloud-api
tags: [Assets, Bans and blocks, Data and memory stores, Generative AI, Luau Execution, Places, Universes, Users]
---

# Cloud / V2 / Universes

Cloud API resource group with 64 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/cloud/v2/universes/{universeId}/secrets` | List Secrets [BETA] |
| `POST` | `/cloud/v2/universes/{universeId}/secrets` | Create Secret [BETA] |
| `GET` | `/cloud/v2/universes/{universeId}/secrets/public-key` | Get Public Key [BETA] |
| `DELETE` | `/cloud/v2/universes/{universeId}/secrets/{secretId}` | Delete Secret [BETA] |
| `PATCH` | `/cloud/v2/universes/{universeId}/secrets/{secretId}` | Update Secret [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}` | Get Universe [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}` | Update Universe [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores` | List Data Stores [STABLE] |
| `DELETE` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}` | Delete Data Store [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries` | List Data Store Entries [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries` | Create Data Store Entry [STABLE] |
| `DELETE` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}` | Delete Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}` | Get Data Store Entry [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}` | Update Data Store Entry [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}:increment` | Increment Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}:listRevisions` | List Data Store Entry Revisions [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries` | List Data Store Entries [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries` | Create Data Store Entry [STABLE] |
| `DELETE` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Delete Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Get Data Store Entry [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Update Data Store Entry [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}:increment` | Increment Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}:listRevisions` | List Data Store Entry Revisions [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}:undelete` | Undelete Data Store [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}/data-stores:snapshot` | Snapshot Data Stores [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/luau-execution-session-task-binary-inputs` | Create Luau Execution Session Task Binary Input [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/memory-store/operations/{operation_id}` | Get Memory Store Flush Operation [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items` | Create Memory Store Queue Item [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items:discard` | Discard Memory Store Queue Items [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items:read` | Read Memory Store Queue Items [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items` | List Memory Store Sorted Map Items [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items` | Create Memory Store Sorted Map Item [STABLE] |
| `DELETE` | `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}` | Delete Memory Store Sorted Map Item [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}` | Get Memory Store Sorted Map Item [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}` | Update Memory Store Sorted Map Item [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/memory-store:flush` | Flush Memory Store [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries` | List Ordered Data Store Entries [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries` | Create Ordered Data Store Entry [STABLE] |
| `DELETE` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Delete Ordered Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Get Ordered Data Store Entry [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}` | Update Ordered Data Store Entry [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}:increment` | Increment Ordered Data Store Entry [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}` | Get Place [STABLE] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/places/{place_id}` | Update Place [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}` | Get Instance [BETA] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}` | Update Instance [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}/operations/{operation_id}` | Get Update Instance Operation [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}:listChildren` | List Instance Children [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}/places/{place_id}/luau-execution-session-tasks` | Create Luau Execution Session Task [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions` | List User Restrictions [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions/{user_restriction_id}` | Get User Restriction [BETA] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions/{user_restriction_id}` | Update User Restriction [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-session-tasks` | Create Luau Execution Session Task [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-sessions/{luau_execution_session_id}/tasks/{task_id}` | Get Luau Execution Session Task [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-sessions/{luau_execution_session_id}/tasks/{task_id}/logs` | List Luau Execution Session Task Logs [STABLE] |
| `GET` | `/cloud/v2/universes/{universe_id}/subscription-products/{subscription_product_id}/subscriptions/{subscription_id}` | Get Subscription [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/user-restrictions` | List User Restrictions [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/user-restrictions/{user_restriction_id}` | Get User Restriction [BETA] |
| `PATCH` | `/cloud/v2/universes/{universe_id}/user-restrictions/{user_restriction_id}` | Update User Restriction [BETA] |
| `GET` | `/cloud/v2/universes/{universe_id}/user-restrictions:listLogs` | List User Restriction Logs [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}:generateSpeechAsset` | Generate Speech Asset [BETA] |
| `POST` | `/cloud/v2/universes/{universe_id}:publishMessage` | Publish Universe Message [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}:restartServers` | Restart Universe Servers [STABLE] |
| `POST` | `/cloud/v2/universes/{universe_id}:translateText` | Translate Text [BETA] |

### `GET` `/cloud/v2/universes/{universeId}/secrets`

**Stability:** BETA

Lists all secrets defined for a universe.
Secret content is not returned for security reasons - only metadata such as ID, domain, creation and update timestamps are included.

Only the owner of the universe can list secrets. For group-owned universes, only the group owner or authorized
members can list secrets.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID
- `limit` (query, integer) - Number of secrets to return per page (1-500, default 10)
- `cursor` (query, string) - Pagination cursor from previous response

**Responses:**

- `200` - OK
- `400` - Bad Request
- `403` - Forbidden

### `POST` `/cloud/v2/universes/{universeId}/secrets`

**Stability:** BETA

Creates a new secret. A maximum of 500 secrets per universe is allowed.
            
Only the owner of the universe can create secrets. For group-owned universes, only the group owner or authorized
members can create secrets.
            
To encrypt the secret:
1. Get the public key using the Get Public Key endpoint
2. Encrypt your secret using LibSodium sealed box
3. Base64 encode the encrypted content

Include the key_id from the public key response in the request.

For an example, see the [Secrets store guide](https://create.roblox.com/docs/cloud/guides/secrets-store).

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID

**Request Body:** The secret to create with encrypted content

**Responses:**

- `201` - Created
- `400` - Bad Request
- `403` - Forbidden
- `409` - Conflict

### `GET` `/cloud/v2/universes/{universeId}/secrets/public-key`

**Stability:** BETA

Retrieves the public key for a universe. You need this key to encrypt secret content 
before sending it to Roblox.

Only the owner of the universe can retrieve the public key. For group-owned universes, only the group owner or
authorized members can retrieve the public key.

The secret id field is static and always returns "public-key".

The returned public key in the secret field is universe-specific and derived from a master key using the universe ID.
Use this key with LibSodium sealed box encryption to encrypt your secret content before 
creating or updating secrets.

Include the key_id from the public key response in the request to create or update a secret.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID

**Responses:**

- `200` - OK
- `400` - Bad Request
- `403` - Forbidden

### `DELETE` `/cloud/v2/universes/{universeId}/secrets/{secretId}`

**Stability:** BETA

Permanently deletes a secret from a universe.

Only the owner of the universe can delete secrets. For group-owned universes, only the group owner or authorized
members can delete secrets.

This operation is irreversible. Make sure you no longer need the secret before deleting it.

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID
- `secretId` (path, string (required)) - The ID of the secret to delete

**Responses:**

- `200` - OK
- `400` - Bad Request
- `403` - Forbidden
- `404` - Not Found

### `PATCH` `/cloud/v2/universes/{universeId}/secrets/{secretId}`

**Stability:** BETA

Updates an existing secret.

Only the owner of the universe can update secrets. For group-owned universes, only the group owner or authorized
members can update secrets.

Only the secret content, key_id, and domain can be updated - the secret ID cannot be changed.

To encrypt the updated secret:
1. Get the current public key using the GetPublicKey endpoint
2. Encrypt your new secret content using LibSodium sealed box
3. Base64 encode the encrypted content

Include the key_id from the public key response in the request.

For an example, see the [Secrets store guide](https://create.roblox.com/docs/cloud/guides/secrets-store).

**Parameters:**

- `universeId` (path, integer (required)) - The universe ID
- `secretId` (path, string (required)) - The ID of the secret to update

**Request Body:** The updated secret data with encrypted content

**Responses:**

- `200` - OK
- `400` - Bad Request
- `403` - Forbidden
- `404` - Not Found

### `GET` `/cloud/v2/universes/{universe_id}`

**Operation:** `Cloud_GetUniverse`

**Stability:** STABLE

Gets the specified universe.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}`

**Operation:** `Cloud_UpdateUniverse`

**Stability:** STABLE

Updates the specified universe.

This method is guaranteed to return all updated fields.
This method may additionally return the full resource.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `updateMask` (query, string) - The list of fields to update.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores`

**Operation:** `Cloud_ListDataStores`

**Stability:** STABLE

Returns a list of data stores.

Data stores scheduled for permanent deletion are omitted from the results
by default (or when `showDeleted` is set to `false`). When this is the
case, the operation will check up to 512 data stores. If all checked data
stores are deleted, it will return an empty list with a page token to
continue iteration.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `maxPageSize` (query, integer) - The maximum number of data stores to return. The service might return fewer than this value. If unspecified, at most 10 data stores are returned. The 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  The `filter` field supports a very small subset of CEL:  * Only the `id` field is su
- `showDeleted` (query, boolean) - If true, resources marked for pending deletion will be included in the results.

**Responses:**

- `200` - OK

### `DELETE` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}`

**Operation:** `Cloud_DeleteDataStore`

**Stability:** BETA

Schedules the specified data store for permanent deletion.

This operation assigns the data store an expiry time 30 days in the future,
at which point permanent deletion begins. To cancel, use the
`UndeleteDataStore` operation before the data store's expiry time.

Permanent deletion consists of deleting all of the entries in the data
store and then the data store resource itself. The data store is no longer
returned by the `ListDataStores` Open Cloud endpoint or
`ListDataStoresAsync` Luau API, and you can reuse the data store's name.

The duration of the permanent deletion process depends on the number of
entries in the data store. However, you can expect a data store with 1
million or fewer entries to be permanently deleted within 3 days.

Data stores scheduled for permanent deletion are returned by the
`ListDataStores` Open Cloud endpoint when the query parameter `showDeleted`
is set to `true`. In the return value, each data store will have a
`DELETED` state and an `expireTime` field...

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries`

**Operation:** `Cloud_ListDataStoreEntries__Using_Universes`

**Stability:** STABLE

Returns a list of entries from a data store.

Only the `path` and `id` fields are populated; use `GetDataStoreEntry`
to retrieve other fields.

Specify the wildcard scope (`-`) to list entries from all scopes.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `maxPageSize` (query, integer) - The maximum number of data store entries to return. The service might return fewer than this value. If unspecified, at most 10 data store entries are 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  The `filter` field supports a very small subset of CEL:  * Only the `id` field is su
- `showDeleted` (query, boolean) - If true, resources marked for pending deletion will be included in the results.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries`

**Operation:** `Cloud_CreateDataStoreEntry__Using_Universes`

**Stability:** STABLE

Creates an entry with the provided ID and value.

Returns a 400 Bad Request if the entry exists.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `id` (query, string) - The ID to use for the data store entry, which will become the final component of the data store entry's resource path.  This value should be a 1-50 ch

**Responses:**

- `200` - OK

### `DELETE` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}`

**Operation:** `Cloud_DeleteDataStoreEntry__Using_Universes_DataStores`

**Stability:** STABLE

Marks the specified entry for deletion.

Entries are not be deleted immediately; instead, the `state` field will
be set to `DELETED`. Permanent deletion occurs after 30 days.

On success, returns 200 OK. If the entry doesn't exist, returns
404 Not Found.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}`

**Operation:** `Cloud_GetDataStoreEntry__Using_Universes_DataStores`

**Stability:** STABLE

Gets the specified entry.

To get the entry at a specific revision, add `@<revisionId>` to the end of
the path.

For example, to get `my-entry` at the revision ID
`08DC3D3F43F9FCC1.0000000001.08DC3D3F43F9FCC1.01`, use the path
`/cloud/v2/universes/1234/data-stores/5678/entries/my-entry@08DC3D3F43F9FCC1.0000000001.08DC3D3F43F9FCC1.01`.

If your entry ID contains one or more `@` characters, and you want to get
the latest version rather than at any specific revision, append the special
revision ID `@latest` to the end of the path. Otherwise, the segment of the
entry ID after the last `@` will be interpreted as a revision ID.

For example, to get the latest revision of `my-entry`, use the path
`/cloud/v2/universes/1234/data-stores/5678/entries/my@entry@latest`.

To get the entry that was current at a specific time, add
`@latest:<timestamp>` to the end of the path, where `<timestamp>` is
RFC-3339 formatted. The given timestamp must be after
the Unix epoch (1/1/1970) and not more than ten mi...

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}`

**Operation:** `Cloud_UpdateDataStoreEntry__Using_Universes_DataStores`

**Stability:** STABLE

Updates the value, attributes, and users of an entry.

Updating specific revisions of the entry is **unsupported**. If you specify
a revision ID in the path and `allow_missing` is `true`, the update request
will instead create a new entry with the `@<revisionId>` suffix as part of
the key.

Partial update is **unsupported**. If attributes or users are not
provided when updating the value, they will be cleared. Value must always
be provided when updating an entry.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `entry_id` (path, string (required)) - The entry ID.
- `allowMissing` (query, boolean) - If set to true, and the data store entry is not found, a data store entry is created.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}:increment`

**Operation:** `Cloud_IncrementDataStoreEntry__Using_Universes_DataStores`

**Stability:** STABLE

Increments the value of the specified entry. Both the existing value and
the increment amount must be integers.

If the entry doesn't exist, creates an entry with the specified value.

Incrementing specific revisions of the entry is **unsupported**. If you
specify a revision ID in the path, the increment request will create a new
entry with the `@<revisionId>` suffix as part of the key.

Known issue: the value may be incremented past the valid range of  values.
When this happens, the returned value will be clamped to the valid range,
but the backend may persist the original value. This behavior is maintained
for backwards compatibility reasons, but may change in a future version of
this API.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/entries/{entry_id}:listRevisions`

**Operation:** `Cloud_ListDataStoreEntryRevisions__Using_Universes_DataStores`

**Stability:** STABLE

List revisions of the data store entry.

This method returns partial data store entries.

In particular, only the `path`, `id`, `createTime`, `revisionCreateTime`,
`revisionId`, `etag`, and `state` fields are populated. Both the `path` and
`id` fields will have an `@<version>` suffix.

In order to get the full entry at a revision, you can use the provided
`path` field with the `GetDataStoreEntry` method, i.e. `GET
/cloud/v2/universes/1234/data-stores/5678/entries/my-entry@<version>`.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `entry_id` (path, string (required)) - The entry ID.
- `maxPageSize` (query, integer) - The maximum number of revisions to return per page.  The service might return fewer than the maximum number of revisions. If unspecified, at most 10 r
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - Supports the following subset of CEL:  * Only the `&&`, `<=`, and `>=` operators are supported. * Only the `revision_create_time` field is supported. 

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries`

**Operation:** `Cloud_ListDataStoreEntries__Using_Universes_DataStores`

**Stability:** STABLE

Returns a list of entries from a data store.

Only the `path` and `id` fields are populated; use `GetDataStoreEntry`
to retrieve other fields.

Specify the wildcard scope (`-`) to list entries from all scopes.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `maxPageSize` (query, integer) - The maximum number of data store entries to return. The service might return fewer than this value. If unspecified, at most 10 data store entries are 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set in order to filter the resources returned.  The `filter` field supports a very small subset of CEL:  * Only the `id` field is su
- `showDeleted` (query, boolean) - If true, resources marked for pending deletion will be included in the results.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries`

**Operation:** `Cloud_CreateDataStoreEntry__Using_Universes_DataStores`

**Stability:** STABLE

Creates an entry with the provided ID and value.

Returns a 400 Bad Request if the entry exists.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `id` (query, string) - The ID to use for the data store entry, which will become the final component of the data store entry's resource path.  This value should be a 1-50 ch

**Responses:**

- `200` - OK

### `DELETE` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_DeleteDataStoreEntry__Using_Universes_DataStores_Scopes`

**Stability:** STABLE

Marks the specified entry for deletion.

Entries are not be deleted immediately; instead, the `state` field will
be set to `DELETED`. Permanent deletion occurs after 30 days.

On success, returns 200 OK. If the entry doesn't exist, returns
404 Not Found.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_GetDataStoreEntry__Using_Universes_DataStores_Scopes`

**Stability:** STABLE

Gets the specified entry.

To get the entry at a specific revision, add `@<revisionId>` to the end of
the path.

For example, to get `my-entry` at the revision ID
`08DC3D3F43F9FCC1.0000000001.08DC3D3F43F9FCC1.01`, use the path
`/cloud/v2/universes/1234/data-stores/5678/entries/my-entry@08DC3D3F43F9FCC1.0000000001.08DC3D3F43F9FCC1.01`.

If your entry ID contains one or more `@` characters, and you want to get
the latest version rather than at any specific revision, append the special
revision ID `@latest` to the end of the path. Otherwise, the segment of the
entry ID after the last `@` will be interpreted as a revision ID.

For example, to get the latest revision of `my-entry`, use the path
`/cloud/v2/universes/1234/data-stores/5678/entries/my@entry@latest`.

To get the entry that was current at a specific time, add
`@latest:<timestamp>` to the end of the path, where `<timestamp>` is
RFC-3339 formatted. The given timestamp must be after
the Unix epoch (1/1/1970) and not more than ten mi...

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_UpdateDataStoreEntry__Using_Universes_DataStores_Scopes`

**Stability:** STABLE

Updates the value, attributes, and users of an entry.

Updating specific revisions of the entry is **unsupported**. If you specify
a revision ID in the path and `allow_missing` is `true`, the update request
will instead create a new entry with the `@<revisionId>` suffix as part of
the key.

Partial update is **unsupported**. If attributes or users are not
provided when updating the value, they will be cleared. Value must always
be provided when updating an entry.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.
- `allowMissing` (query, boolean) - If set to true, and the data store entry is not found, a data store entry is created.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}:increment`

**Operation:** `Cloud_IncrementDataStoreEntry__Using_Universes_DataStores_Scopes`

**Stability:** STABLE

Increments the value of the specified entry. Both the existing value and
the increment amount must be integers.

If the entry doesn't exist, creates an entry with the specified value.

Incrementing specific revisions of the entry is **unsupported**. If you
specify a revision ID in the path, the increment request will create a new
entry with the `@<revisionId>` suffix as part of the key.

Known issue: the value may be incremented past the valid range of  values.
When this happens, the returned value will be clamped to the valid range,
but the backend may persist the original value. This behavior is maintained
for backwards compatibility reasons, but may change in a future version of
this API.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}/scopes/{scope_id}/entries/{entry_id}:listRevisions`

**Operation:** `Cloud_ListDataStoreEntryRevisions__Using_Universes_DataStores_Scopes`

**Stability:** STABLE

List revisions of the data store entry.

This method returns partial data store entries.

In particular, only the `path`, `id`, `createTime`, `revisionCreateTime`,
`revisionId`, `etag`, and `state` fields are populated. Both the `path` and
`id` fields will have an `@<version>` suffix.

In order to get the full entry at a revision, you can use the provided
`path` field with the `GetDataStoreEntry` method, i.e. `GET
/cloud/v2/universes/1234/data-stores/5678/entries/my-entry@<version>`.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.
- `maxPageSize` (query, integer) - The maximum number of revisions to return per page.  The service might return fewer than the maximum number of revisions. If unspecified, at most 10 r
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - Supports the following subset of CEL:  * Only the `&&`, `<=`, and `>=` operators are supported. * Only the `revision_create_time` field is supported. 

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores/{data_store_id}:undelete`

**Operation:** `Cloud_UndeleteDataStore`

**Stability:** BETA

Restore the data store

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `data_store_id` (path, string (required)) - The data-store ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/data-stores:snapshot`

**Operation:** `Cloud_SnapshotDataStores`

**Stability:** STABLE

Takes a new snapshot of the data stores in an experience.

After a snapshot, the next write to every key in the experience will
create a versioned backup of the previous data, regardless of the time of
the last write.

In effect, all data current at the time of the snapshot is guaranteed to be
available as a versioned backup for at least 30 days.

Snapshots can be taken once per UTC day, per experience. If the latest
snapshot was taken within the same UTC day, this operation is a no-op and
the time of the latest snapshot will be returned.

For more information on using snapshots, see the [Data
stores](https://create.roblox.com/docs/cloud-services/data-stores#snapshots)
Engine guide.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/luau-execution-session-task-binary-inputs`

**Operation:** `Cloud_CreateLuauExecutionSessionTaskBinaryInput`

**Stability:** STABLE

Create a new `LuauExecutionSessionTaskBinaryInput`.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/memory-store/operations/{operation_id}`

**Operation:** `Cloud_GetMemoryStoreFlushOperation`

**Stability:** BETA

Retrieves the status of the operation to [flush the memory stores of a universe](https://create.roblox.com/docs/cloud/reference/features/storage#Cloud_FlushMemoryStore).

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `operation_id` (path, string (required)) - The operation ID.
- `scope` (query, string) - The scope of the memory store flush operation.  Possible values:    | Value | Description |   | --- | --- |   | LIVE |  Flush the live memory store sc

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items`

**Operation:** `Cloud_CreateMemoryStoreQueueItem`

**Stability:** STABLE

Creates a new queue item.

If `ttl` is set, the item will automatically be removed from the queue
after the time interval specified.

If a numerical `priority` is set, the item will be inserted into the queue
based on the priority value. The higher the value, the closer to the front
of the queue the item will be. If priority values are the same then the
item will be inserted after existing values with the same priority.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `queue_id` (path, string (required)) - The queue ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items:discard`

**Operation:** `Cloud_DiscardMemoryStoreQueueItems`

**Stability:** STABLE

Discards read items from the front of the queue.

Takes a `readId` from a previous `Read` operation.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `queue_id` (path, string (required)) - The queue ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/memory-store/queues/{queue_id}/items:read`

**Operation:** `Cloud_ReadMemoryStoreQueueItems`

**Stability:** STABLE

Returns the specified number of items at the front of the queue.



**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `queue_id` (path, string (required)) - The queue ID.
- `count` (query, integer) - The number of items to read from the queue If unspecified, 1 item will be returned. The maximum value is 200; values above 200 will be coerced to 200.
- `allOrNothing` (query, boolean) - If `all_or_nothing` is true and the requested number of objects is not available, will return a 404 Error.  Otherwise, will return the path and read_i
- `invisibilityWindow` (query, string) - Invisibility window for items read, in seconds.  Items read are invisible in subsequent reads during the invisibility window duration.  It must be wri

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items`

**Operation:** `Cloud_ListMemoryStoreSortedMapItems`

**Stability:** STABLE

Gets and returns items in the map with a given order and filter.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `sorted_map_id` (path, string (required)) - The sorted-map ID.
- `maxPageSize` (query, integer) - The maximum number of memory store sorted map items to return. The service might return fewer than this value. If unspecified, at most 1 memory store 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `orderBy` (query, string) - If specified, results are ordered according to the specified fields.  Values must be a comma-separated list of fields, with an optional, per-field " d
- `filter` (query, string) - This field may be set in order to filter the resources returned.  Filtering conforms to Common Expression Language (CEL). Only the `id` and `sortKey` 

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items`

**Operation:** `Cloud_CreateMemoryStoreSortedMapItem`

**Stability:** STABLE

Creates the specified map item if it doesn't exist.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `sorted_map_id` (path, string (required)) - The sorted-map ID.
- `id` (query, string) - The ID to use for the memory store sorted map item, which will become the final component of the memory store sorted map item's resource path.  This v

**Responses:**

- `200` - OK

### `DELETE` `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}`

**Operation:** `Cloud_DeleteMemoryStoreSortedMapItem`

**Stability:** STABLE

Deletes the specified item from the map.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `sorted_map_id` (path, string (required)) - The sorted-map ID.
- `item_id` (path, string (required)) - The item ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}`

**Operation:** `Cloud_GetMemoryStoreSortedMapItem`

**Stability:** STABLE

Gets and returns the value of the given key in the map.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `sorted_map_id` (path, string (required)) - The sorted-map ID.
- `item_id` (path, string (required)) - The item ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/memory-store/sorted-maps/{sorted_map_id}/items/{item_id}`

**Operation:** `Cloud_UpdateMemoryStoreSortedMapItem`

**Stability:** STABLE

Updates the specified map item.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `sorted_map_id` (path, string (required)) - The sorted-map ID.
- `item_id` (path, string (required)) - The item ID.
- `allowMissing` (query, boolean) - If set to true, and the memory store sorted map item is not found, a memory store sorted map item is created.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/memory-store:flush`

**Operation:** `Cloud_FlushMemoryStore`

**Stability:** STABLE

Asynchronously flush all data structures in the universe.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `scope` (query, string) - The scope of the memory store to flush.  Possible values:    | Value | Description |   | --- | --- |   | LIVE |  Flush the live memory store scope. Th

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries`

**Operation:** `Cloud_ListOrderedDataStoreEntries`

**Stability:** STABLE

Returns a list of entries from an ordered data store.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `maxPageSize` (query, integer) - The maximum number of ordered data store entries to return. The service might return fewer than this value. If unspecified, at most 10 ordered data st
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `orderBy` (query, string) - If specified, results are ordered according to the specified fields.  Values must be a comma-separated list of fields, with an optional, per-field " d
- `filter` (query, string) - This field may be set in order to filter the resources returned.  We support two comparison operators for this operation: `<=` and `>=`.These comparis

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries`

**Operation:** `Cloud_CreateOrderedDataStoreEntry`

**Stability:** STABLE

Creates an entry with the provided ID and value.

Returns a 400 Bad Request if the entry exists.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `id` (query, string) - The ID to use for the ordered data store entry, which will become the final component of the ordered data store entry's resource path.  This value sho

**Responses:**

- `200` - OK

### `DELETE` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_DeleteOrderedDataStoreEntry`

**Stability:** STABLE

Deletes the specified entry.

On success, returns 200 OK. If the entry doesn't exist, returns
404 Not Found.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_GetOrderedDataStoreEntry`

**Stability:** STABLE

Gets the specified entry.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}`

**Operation:** `Cloud_UpdateOrderedDataStoreEntry`

**Stability:** STABLE

Updates the value of an entry.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.
- `allowMissing` (query, boolean) - If set to true, and the ordered data store entry is not found, a ordered data store entry is created.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/ordered-data-stores/{ordered_data_store_id}/scopes/{scope_id}/entries/{entry_id}:increment`

**Operation:** `Cloud_IncrementOrderedDataStoreEntry`

**Stability:** STABLE

Increments the value of the specified entry. Both the existing value and
the increment amount must be integers.

If the entry doesn't exist, creates an entry with the specified value.

Known issue: the value may be incremented past the valid range of  values.
When this happens, the returned value will be clamped to the valid range,
but the backend may persist the original value. This behavior is maintained
for backwards compatibility reasons, but may change in a future version of
this API.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `ordered_data_store_id` (path, string (required)) - The ordered-data-store ID.
- `scope_id` (path, string (required)) - The scope ID.
- `entry_id` (path, string (required)) - The entry ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}`

**Operation:** `Cloud_GetPlace`

**Stability:** STABLE

Gets the specified place.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/places/{place_id}`

**Operation:** `Cloud_UpdatePlace`

**Stability:** STABLE

Updates the specified place.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `updateMask` (query, string) - The list of fields to update.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}`

**Operation:** `Cloud_GetInstance`

**Stability:** BETA

Gets an instance and its property data.

The maximum supported response data size is 500,000 bytes. If this limit is
exceeded, the returned `Operation` will be completed with an error result
that has an error code of `422`.


**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `instance_id` (path, string (required)) - The instance ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}`

**Operation:** `Cloud_UpdateInstance`

**Stability:** BETA

Updates an instance's property data.

When updating a `Script` instance's source property, the maximum supported
property size is 200,000 bytes after UTF-8 encoding.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `instance_id` (path, string (required)) - The instance ID.
- `updateMask` (query, string) - The list of fields to update.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}/operations/{operation_id}`

**Operation:** `Cloud_GetUpdateInstanceOperation`

**Stability:** BETA

Retrieves the status of the operation to [update an instance](https://create.roblox.com/docs/cloud/reference/features/universes#Cloud_UpdateInstance).

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `instance_id` (path, string (required)) - The instance ID.
- `operation_id` (path, string (required)) - The operation ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/instances/{instance_id}:listChildren`

**Operation:** `Cloud_ListInstanceChildren`

**Stability:** BETA

Lists an instance's children.

The maximum supported response data size is 500,000 bytes. If this limit is
exceeded, the returned `Operation` will be completed with an error result
that has an error code of `422`.



**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `instance_id` (path, string (required)) - The instance ID.
- `maxPageSize` (query, integer) - The maximum number of child instance to return. The service may return fewer than this value. If unspecified, at most 200 children will be returned. T
- `pageToken` (query, string) - A page token, received from a previous `ListInstanceChildrenRequest` call. Provide this to retrieve the subsequent page.  When paginating, all other p

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/places/{place_id}/luau-execution-session-tasks`

**Operation:** `Cloud_CreateLuauExecutionSessionTask__Using_Universes`

**Stability:** STABLE

Creates a task but does not wait for the task to complete.

To check whether a task has
completed, call the `GetLuauExecutionSessionTask` method and inspect the
`state` field of the returned resource.

Quotas:
* 5 calls per minute per API key owner
* 45 calls per minute per IP address

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions`

**Operation:** `Cloud_ListUserRestrictions__Using_Universes`

**Stability:** BETA

List user restrictions for users that have ever been banned in either a
universe or a specific place.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `maxPageSize` (query, integer) - The maximum number of user restrictions to return. The service might return fewer than this value. If unspecified, at most 10 user restrictions are re
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions/{user_restriction_id}`

**Operation:** `Cloud_GetUserRestriction__Using_Universes_Places`

**Stability:** BETA

Get the user restriction.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `user_restriction_id` (path, string (required)) - The user-restriction ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/places/{place_id}/user-restrictions/{user_restriction_id}`

**Operation:** `Cloud_UpdateUserRestriction__Using_Universes_Places`

**Stability:** BETA

Update the user restriction.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `user_restriction_id` (path, string (required)) - The user-restriction ID.
- `updateMask` (query, string) - The list of fields to update.  The `game_join_restriction` field must be updated atomically; field masks that index into `game_join_restriction` (such
- `idempotencyKey.key` (query, string) - The unique key to use for idempotency.
- `idempotencyKey.firstSent` (query, string) - The timestamp at which the first request was sent.  If this is further in the past than the lifetime of the idempotency key (which *may* exceed the an

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-session-tasks`

**Operation:** `Cloud_CreateLuauExecutionSessionTask__Using_Universes_Places`

**Stability:** STABLE

Creates a task but does not wait for the task to complete.

To check whether a task has
completed, call the `GetLuauExecutionSessionTask` method and inspect the
`state` field of the returned resource.

Quotas:
* 5 calls per minute per API key owner
* 45 calls per minute per IP address

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `version_id` (path, string (required)) - The version ID.

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-sessions/{luau_execution_session_id}/tasks/{task_id}`

**Operation:** `Cloud_GetLuauExecutionSessionTask`

**Stability:** STABLE

Gets information about a task.

Quotas:
* 45 calls per minute per API key owner or IP address

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `version_id` (path, string (required)) - The version ID.
- `luau_execution_session_id` (path, string (required)) - The luau-execution-session ID.
- `task_id` (path, string (required)) - The task ID.
- `view` (query, string) - The view in which to retrieve the luau execution session task.  Supports BASIC and FULL.  Defaults to BASIC.  Possible values:    | Value | Descriptio

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/places/{place_id}/versions/{version_id}/luau-execution-sessions/{luau_execution_session_id}/tasks/{task_id}/logs`

**Operation:** `Cloud_ListLuauExecutionSessionTaskLogs`

**Stability:** STABLE

Lists log chunks generated by a `LuauExecutionSessionTask`.

Quotas:
* 45 calls per minute per API key owner or IP address

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `place_id` (path, string (required)) - The place ID.
- `version_id` (path, string (required)) - The version ID.
- `luau_execution_session_id` (path, string (required)) - The luau-execution-session ID.
- `task_id` (path, string (required)) - The task ID.
- `maxPageSize` (query, integer) - The maximum number of luau execution session task logs to return. The service might return fewer than this value. If unspecified, at most 10000 luau e
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `view` (query, string) - The view in which to retrieve the luau execution session task log.  Supports FLAT and STRUCTURED.  Defaults to FLAT.  Possible values:    | Value | De

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/subscription-products/{subscription_product_id}/subscriptions/{subscription_id}`

**Operation:** `Cloud_GetSubscription`

**Stability:** BETA

Get the subscription.

The `universe.subscription-product.subscription:read` scope only allows
reading subscriptions of the user making the request. Because of this, the
subscription ID must match the user ID of the user making the request. Note
that this scope might be more relevant for OAuth 2.0 apps.

To read all subscriptions made by users for a particular universe, use the
`universe:write` scope instead.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `subscription_product_id` (path, string (required)) - The subscription-product ID.
- `subscription_id` (path, string (required)) - The subscription ID.
- `view` (query, string) - The view in which to retrieve the subscription.  Supports BASIC and FULL.  Defaults to BASIC.  Possible values:    | Value | Description |   | --- | -

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/user-restrictions`

**Operation:** `Cloud_ListUserRestrictions`

**Stability:** BETA

List user restrictions for users that have ever been banned in either a
universe or a specific place.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `maxPageSize` (query, integer) - The maximum number of user restrictions to return. The service might return fewer than this value. If unspecified, at most 10 user restrictions are re
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/user-restrictions/{user_restriction_id}`

**Operation:** `Cloud_GetUserRestriction__Using_Universes`

**Stability:** BETA

Get the user restriction.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `user_restriction_id` (path, string (required)) - The user-restriction ID.

**Responses:**

- `200` - OK

### `PATCH` `/cloud/v2/universes/{universe_id}/user-restrictions/{user_restriction_id}`

**Operation:** `Cloud_UpdateUserRestriction__Using_Universes`

**Stability:** BETA

Update the user restriction.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `user_restriction_id` (path, string (required)) - The user-restriction ID.
- `updateMask` (query, string) - The list of fields to update.  The `game_join_restriction` field must be updated atomically; field masks that index into `game_join_restriction` (such
- `idempotencyKey.key` (query, string) - The unique key to use for idempotency.
- `idempotencyKey.firstSent` (query, string) - The timestamp at which the first request was sent.  If this is further in the past than the lifetime of the idempotency key (which *may* exceed the an

**Responses:**

- `200` - OK

### `GET` `/cloud/v2/universes/{universe_id}/user-restrictions:listLogs`

**Operation:** `Cloud_ListUserRestrictionLogs`

**Stability:** BETA

List changes to UserRestriction resources within a given universe.
This includes both universe-level and place-level restrictions.

For universe-level restriction logs, the `place` field will be empty.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.
- `maxPageSize` (query, integer) - The maximum number of UserRestrictionLogs to return. The service may return fewer than this value. If unspecified, at most 10 UserRestrictionLogs are 
- `pageToken` (query, string) - A page token, received from a previous call, to retrieve a subsequent page.  When paginating, all other parameters provided to the subsequent call mus
- `filter` (query, string) - This field may be set to filter the logs returned.  The `filter` field supports a very small number of CEL:  * `user` * `place` * The `==` comparison 

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}:generateSpeechAsset`

**Operation:** `Cloud_GenerateSpeechAsset`

**Stability:** BETA

Generates an English speech audio asset from the specified text.

This endpoint requires the `asset:read` and `asset:write` scopes in
addition to the `universe:write` scope.

The response returns an `Operation` object that must be prefixed with
`/assets/v1`. For example, the URL to discover the result of the operation
could be
`https://apis.roblox.com/assets/v1/operations/8b42ef30-9c17-4526-b8cf-2ff0136ca94d`.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}:publishMessage`

**Operation:** `Cloud_PublishUniverseMessage`

**Stability:** STABLE

Publishes a message to the universe's live servers.

Servers can consume messages via
[MessagingService](https://create.roblox.com/docs/reference/engine/classes/MessagingService).

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}:restartServers`

**Operation:** `Cloud_RestartUniverseServers`

**Stability:** STABLE

Restarts active servers for a specific universe. Defaults to only
restarting servers running older versions, but can be configured to restart
all servers regardless of version. Used for releasing experience updates.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK

### `POST` `/cloud/v2/universes/{universe_id}:translateText`

**Operation:** `Cloud_TranslateText`

**Stability:** BETA

Translates the provided text from one language to another.

**Parameters:**

- `universe_id` (path, string (required)) - The universe ID.

**Responses:**

- `200` - OK
