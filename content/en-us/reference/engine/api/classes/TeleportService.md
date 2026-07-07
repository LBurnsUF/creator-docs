---
title: TeleportService
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# TeleportService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.TeleportService.CustomizedTeleportUI` | `bool` | [NotReplicated] [Deprecated] |

## Methods

### `Class.TeleportService:Block`

``Block()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:GetArrivingTeleportGui`

``GetArrivingTeleportGui()`` → `Class.Instance`

### `Class.TeleportService:GetLocalPlayerTeleportData`

``GetLocalPlayerTeleportData()`` → `Variant`

### `Class.TeleportService:GetPlayerPlaceInstanceAsync`

``GetPlayerPlaceInstanceAsync(userId: `Datatype.User`)`` → `Tuple`
  [Yields]

### `Class.TeleportService:GetTeleportSetting`

``GetTeleportSetting(setting: `string`)`` → `Variant`

### `Class.TeleportService:GetThirdPartyTeleportInfo`

``GetThirdPartyTeleportInfo(goForth: `bool`)`` → `Tuple`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:PromptExperienceDetailsAsync`

``PromptExperienceDetailsAsync(player: `Class.Player`, universeId: `int64`)`` → `Enum.PromptExperienceDetailsResult`
  [Yields]

### `Class.TeleportService:PromptExperienceDetailsCompleted`

``PromptExperienceDetailsCompleted(resultEnum: `Enum.PromptExperienceDetailsResult`, errorMessage: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:ReserveServer`

``ReserveServer(placeId: `int64`)`` → `Tuple`
  [Yields] [Deprecated]

### `Class.TeleportService:ReserveServerAsync`

``ReserveServerAsync(placeId: `int64`)`` → `Tuple`
  [Yields]

### `Class.TeleportService:SetTeleportGui`

``SetTeleportGui(gui: `Class.Instance`)`` → `null`

### `Class.TeleportService:SetTeleportSetting`

``SetTeleportSetting(setting: `string`, value: `Variant`)`` → `null`

### `Class.TeleportService:Teleport`

``Teleport(placeId: `int64`, player: `Class.Instance`, teleportData: `Variant`, customLoadingScreen: `Class.Instance`)`` → `null`

### `Class.TeleportService:TeleportAsync`

``TeleportAsync(placeId: `int64`, players: `Datatype.Instances`, teleportOptions: `Class.Instance`)`` → `Class.Instance`
  [Yields]

### `Class.TeleportService:TeleportCancel`

``TeleportCancel()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:TeleportPartyAsync`

``TeleportPartyAsync(placeId: `int64`, players: `Datatype.Instances`, teleportData: `Variant`, customLoadingScreen: `Class.Instance`)`` → `string`
  [Yields]

### `Class.TeleportService:TeleportReconnect`

``TeleportReconnect()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:TeleportToPlaceInstance`

``TeleportToPlaceInstance(placeId: `int64`, instanceId: `string`, player: `Class.Instance`, spawnName: `string`, teleportData: `Variant`, customLoadingScreen: `Class.Instance`)`` → `null`

### `Class.TeleportService:TeleportToPrivateServer`

``TeleportToPrivateServer(placeId: `int64`, reservedServerAccessCode: `string`, players: `Datatype.Instances`, spawnName: `string`, teleportData: `Variant`, customLoadingScreen: `Class.Instance`)`` → `null`

### `Class.TeleportService:TeleportToSpawnByName`

``TeleportToSpawnByName(placeId: `int64`, spawnName: `string`, player: `Class.Instance`, teleportData: `Variant`, customLoadingScreen: `Class.Instance`)`` → `null`

### `Class.TeleportService:TeleportTrustedBackForth`

``TeleportTrustedBackForth(goForth: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:TeleportTrustedBackHistory`

``TeleportTrustedBackHistory(placeId: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:TeleportedPlacesBackHistory`

``TeleportedPlacesBackHistory()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:TeleportedUniversesBackHistory`

``TeleportedUniversesBackHistory()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.TeleportService:UnblockAsync`

``UnblockAsync()`` → `Tuple`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.TeleportService.LocalPlayerArrivedFromTeleport`

Fires with: (loadingGui: `Class.Instance`, dataTable: `Variant`)

### `Class.TeleportService.MenuTeleportAttempt`

Fires with: ()

### `Class.TeleportService.OpenExperienceDetailsPrompt`

Fires with: (universeId: `int64`)

### `Class.TeleportService.ReconnectTeleportInitFailed`

Fires with: (player: `Class.Instance`, teleportResult: `Enum.TeleportResult`, errorMessage: `string`, placeId: `int64`, teleportOptions: `Class.Instance`)

### `Class.TeleportService.TeleportInitFailed`

Fires with: (player: `Class.Instance`, teleportResult: `Enum.TeleportResult`, errorMessage: `string`, placeId: `int64`, teleportOptions: `Class.Instance`)
