---
title: StudioPublishService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioPublishService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **PublishLocked**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **ClearUploadNames**() -> `null`
- **CloseAfterPublish**(`closeMode: StudioCloseMode`) -> `null`
- **PublishAs**(`universeId: int64`, `placeId: int64`, `groupId: int64`, `isPublish: bool`, `publishParameters: Variant`, `willRetryOnConflict: bool = false`, `allowOpeningNewPlace: bool = true`) -> `null`
- **PublishThenTurnOnTeamCreate**() -> `null`
- **RefreshDocumentDisplayName**() -> `null`
- **RegisterPublishHold**(`priority: int`, `callback: Function`) -> `RBXScriptConnection`
- **SaveOrPublishPlaceToRobloxIsCanceled**() -> `null`
- **SetTeamCreateOnPublishInfo**(`shouldTurnOnTcOnPublish: bool`, `newPlaceName: string`) -> `null`
- **SetUniverseDisplayName**(`newName: string`) -> `null`
- **SetUploadNames**(`placeName: string`, `universeName: string`) -> `null`
- **ShowSaveOrPublishPlaceToRoblox**(`showGameSelect: bool`, `isPublish: bool`, `closeMode: StudioCloseMode`) -> `null`

## Events

- **GameNameUpdated**(`name: string`)
- **GamePublishCancelled**()
- **GamePublishFinished**(`success: bool`, `gameId: int64`, `message: string`, `reason: StudioPlaceUpdateFailureReason`)
- **OnPublishAttempt**(`isPublishAs: bool`)
- **OnSaveOrPublishPlaceToRoblox**(`showGameSelect: bool`, `isPublish: bool`, `closeMode: StudioCloseMode`)
