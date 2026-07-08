---
title: V1 / Automatic Translation / Languages
type: cloud-api
tags: [Localization]
---

# V1 / Automatic Translation / Languages

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/automatic-translation/languages/{languageCode}/target-languages` | Checks if the requested target languages are allowed for automatic translation based on the source l |

### `GET` `/v1/automatic-translation/languages/{languageCode}/target-languages`

**Parameters:**

- `languageCode` (path, string (required)) - The source language.
- `targetLanguages` (query, array) - Optional target languages. If not passed in, all allowed target languages for the source language will be returned.
- `gameId` (query, integer) - Optional gameId. If not passed in, we'll return the default list of languages allowed.

**Responses:**

- `200` - OK
- `400` - 73: Maximum languages exceeded. Please keep the number of languages per request below the maximum. 
- `503` - 17: Feature is disabled
