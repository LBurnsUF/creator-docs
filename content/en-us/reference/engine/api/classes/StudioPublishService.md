---
title: StudioPublishService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioPublishService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StudioPublishService.PublishLocked` | `bool` |  {security: RobloxScriptSecurity} |

## Methods

### `Class.StudioPublishService:ClearUploadNames`

``ClearUploadNames()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:CloseAfterPublish`

``CloseAfterPublish(closeMode: `Enum.StudioCloseMode`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:PublishAs`

``PublishAs(universeId: `int64`, placeId: `int64`, groupId: `int64`, isPublish: `bool`, publishParameters: `Variant`, willRetryOnConflict: `bool`, allowOpeningNewPlace: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:PublishThenTurnOnTeamCreate`

``PublishThenTurnOnTeamCreate()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:RefreshDocumentDisplayName`

``RefreshDocumentDisplayName()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:RegisterPublishHold`

``RegisterPublishHold(priority: `int`, callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:SaveOrPublishPlaceToRobloxIsCanceled`

``SaveOrPublishPlaceToRobloxIsCanceled()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:SetTeamCreateOnPublishInfo`

``SetTeamCreateOnPublishInfo(shouldTurnOnTcOnPublish: `bool`, newPlaceName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:SetUniverseDisplayName`

``SetUniverseDisplayName(newName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:SetUploadNames`

``SetUploadNames(placeName: `string`, universeName: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.StudioPublishService:ShowSaveOrPublishPlaceToRoblox`

``ShowSaveOrPublishPlaceToRoblox(showGameSelect: `bool`, isPublish: `bool`, closeMode: `Enum.StudioCloseMode`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.StudioPublishService.GameNameUpdated`

Fires with: (name: `string`)

### `Class.StudioPublishService.GamePublishCancelled`

Fires with: ()

### `Class.StudioPublishService.GamePublishFinished`

Fires with: (success: `bool`, gameId: `int64`, message: `string`, reason: `Enum.StudioPlaceUpdateFailureReason`)

### `Class.StudioPublishService.OnPublishAttempt`

Fires with: (isPublishAs: `bool`)

### `Class.StudioPublishService.OnSaveOrPublishPlaceToRoblox`

Fires with: (showGameSelect: `bool`, isPublish: `bool`, closeMode: `Enum.StudioCloseMode`)
