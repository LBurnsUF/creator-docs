---
title: Matchmaking Api / V1 / Matchmaking
type: cloud-api
tags: [Matchmaking]
---

# Matchmaking Api / V1 / Matchmaking

Cloud API resource group with 22 endpoint(s).

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| `POST` | `/matchmaking-api/v1/matchmaking/player-attribute` | Create a PlayerAttributeDefinition. [BETA] |
| `DELETE` | `/matchmaking-api/v1/matchmaking/player-attribute/{attributeId}` | Delete the PlayerAttributeDefinition specified by attributeId. [BETA] |
| `PATCH` | `/matchmaking-api/v1/matchmaking/player-attribute/{attributeId}` | Update the PlayerAttributeDefinition specified by attributeId. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/player-attributes/{universeId}` | List all PlayerAttributeDefinitions of a universe. [BETA] |
| `POST` | `/matchmaking-api/v1/matchmaking/scoring-configuration` | Creates a matchmaking scoring configuration. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/scoring-configuration/default-weights` |  [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/scoring-configuration/generate-mock-servers` |  [BETA] |
| `POST` | `/matchmaking-api/v1/matchmaking/scoring-configuration/place` | Sets a matchmaking scoring configuration for a place. [BETA] |
| `DELETE` | `/matchmaking-api/v1/matchmaking/scoring-configuration/place/{placeId}` | Removes the matchmaking scoring configuration for a place. [BETA] |
| `DELETE` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}` | Deletes a matchmaking scoring configuration. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}` | Updates a matchmaking scoring configuration. [BETA] |
| `PATCH` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}` | Updates a matchmaking scoring configuration. [BETA] |
| `POST` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals` | Creates a matchmaking scoring configuration signal. [BETA] |
| `DELETE` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals/{signalName}` | Deletes a matchmaking scoring configuration custom signal. [BETA] |
| `PATCH` | `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals/{signalName}` | Updates a matchmaking scoring configuration signal. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/scoring-configurations/{universeId}` | List all matchmaking scoring configurations for a universe. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/scoring-configurations/{universeId}/places` | List all places with a matchmaking scoring configuration for a universe. [BETA] |
| `POST` | `/matchmaking-api/v1/matchmaking/server-attribute` | Create a ServerAttributeDefinition. [BETA] |
| `DELETE` | `/matchmaking-api/v1/matchmaking/server-attribute/{attributeId}` | Delete the ServerAttributeDefinition specified by attributeId. [BETA] |
| `PATCH` | `/matchmaking-api/v1/matchmaking/server-attribute/{attributeId}` | Update the ServerAttributeDefinition specified by attributeId. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/server-attributes/{universeId}` | List all ServerAttributeDefinitions of a universe. [BETA] |
| `GET` | `/matchmaking-api/v1/matchmaking/universe/{universeId}/feature-flags` | Gets feature flags for a customized matchmaking for a given universe. [BETA] |

### `POST` `/matchmaking-api/v1/matchmaking/player-attribute`

**Stability:** BETA

**Responses:**

- `200` - Success

### `DELETE` `/matchmaking-api/v1/matchmaking/player-attribute/{attributeId}`

**Stability:** BETA

**Parameters:**

- `attributeId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/matchmaking-api/v1/matchmaking/player-attribute/{attributeId}`

**Stability:** BETA

**Parameters:**

- `attributeId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/player-attributes/{universeId}`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/matchmaking/scoring-configuration`

**Stability:** BETA

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/scoring-configuration/default-weights`

**Stability:** BETA

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/scoring-configuration/generate-mock-servers`

**Stability:** BETA

**Parameters:**

- `count` (query, integer) - 
- `capacity` (query, integer) - 
- `playerAge` (query, integer) - 
- `playerPlayHistory` (query, number) - 
- `isPlayerVoiceChatEnabled` (query, boolean) - 

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/matchmaking/scoring-configuration/place`

**Stability:** BETA

**Responses:**

- `200` - Success

### `DELETE` `/matchmaking-api/v1/matchmaking/scoring-configuration/place/{placeId}`

**Stability:** BETA

**Parameters:**

- `placeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `DELETE` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `DELETE` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals/{signalName}`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 
- `signalName` (path, string (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/matchmaking-api/v1/matchmaking/scoring-configuration/{scoringConfigurationId}/signals/{signalName}`

**Stability:** BETA

**Parameters:**

- `scoringConfigurationId` (path, string (required)) - 
- `signalName` (path, string (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/scoring-configurations/{universeId}`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/scoring-configurations/{universeId}/places`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `POST` `/matchmaking-api/v1/matchmaking/server-attribute`

**Stability:** BETA

**Responses:**

- `200` - Success

### `DELETE` `/matchmaking-api/v1/matchmaking/server-attribute/{attributeId}`

**Stability:** BETA

**Parameters:**

- `attributeId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `PATCH` `/matchmaking-api/v1/matchmaking/server-attribute/{attributeId}`

**Stability:** BETA

**Parameters:**

- `attributeId` (path, string (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/server-attributes/{universeId}`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success

### `GET` `/matchmaking-api/v1/matchmaking/universe/{universeId}/feature-flags`

**Stability:** BETA

**Parameters:**

- `universeId` (path, integer (required)) - 

**Responses:**

- `200` - Success
