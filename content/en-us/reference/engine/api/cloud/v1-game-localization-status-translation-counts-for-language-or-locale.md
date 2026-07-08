---
title: V1 / Game Localization Status / Translation Counts For Language Or Locale
type: cloud-api
tags: [Localization, Universes]
---

# V1 / Game Localization Status / Translation Counts For Language Or Locale

Cloud API resource group with 1 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `GET` | `/v1/game-localization-status/translation-counts-for-language-or-locale` | Gets the language translation counts for the specified table. The languages to retrieve must be pro |

### `GET` `/v1/game-localization-status/translation-counts-for-language-or-locale`

**Parameters:**

- `gameIds` (query, array (required)) - List of game ids to retrieve translation counts for.
- `languageOrLocaleCode` (query, string (required)) - The code for the language or locale.
- `languageOrLocaleType` (query, string (required)) - Indicates whether the languageOrLocaleCode represents a language or locale.

**Responses:**

- `200` - OK
- `400` - 66: Games can't be null or empty 67: Maximum games exceeded. Please keep the number of games per re
- `401` - 0: Authorization has been denied for this request.
