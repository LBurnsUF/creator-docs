---
title: V2 / Compression Dictionaries
type: cloud-api
tags: [Metadata]
---

# V2 / Compression Dictionaries

Cloud API resource group with 2 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v2/compression-dictionaries` | Returns a listing of all known compression dictionaries, including their SHA256 and creation date.  |
| `GET` | `/v2/compression-dictionaries/{dictionarySha256}` | Returns the specified compression dictionary as a file download. |

### `GET` `/v2/compression-dictionaries`

**Responses:**

- `200` - OK

### `GET` `/v2/compression-dictionaries/{dictionarySha256}`

**Parameters:**

- `dictionarySha256` (path, string (required)) - The SHA256 of the dictionary we wish to download.

**Responses:**

- `200` - OK
