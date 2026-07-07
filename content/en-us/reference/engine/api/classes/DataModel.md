---
title: DataModel
type: class
superclass: ServiceProvider
tags: [NotCreatable]
---

# DataModel

**Inherits**: ServiceProvider > Instance > Object

**Tags**: NotCreatable

## Properties

- **CreatorId**: `int64` [ReadOnly] [NotReplicated]
- **CreatorType**: `CreatorType` [ReadOnly] [NotReplicated]
- **Environment**: `string` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **GameId**: `int64` [ReadOnly] [NotReplicated]
- **GearGenreSetting**: `GearGenreSetting` [ReadOnly] [NotReplicated] [Deprecated]
- **Genre**: `Genre` [ReadOnly] [NotReplicated]
- **IsSFFlagsLoaded**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **JobId**: `string` [ReadOnly] [NotReplicated]
- **MatchmakingType**: `MatchmakingType` [ReadOnly] [NotReplicated]
- **PlaceId**: `int64` [ReadOnly] [NotReplicated]
- **PlaceVersion**: `int` [ReadOnly] [NotReplicated]
- **PrivateServerId**: `string` [ReadOnly] [NotReplicated]
- **PrivateServerOwnerId**: `int64` [ReadOnly] [NotReplicated]
- **RunService**: `RunService` [ReadOnly] [NotReplicated]
- **VIPServerId**: `string` [Hidden] [ReadOnly] [NotReplicated] [Deprecated]
- **VIPServerOwnerId**: `int64` [Hidden] [ReadOnly] [NotReplicated] [Deprecated]
- **Workspace**: `Workspace` [ReadOnly] [NotReplicated]
- **lighting**: `Instance` [ReadOnly] [NotReplicated] [Deprecated]
- **workspace**: `Workspace` [ReadOnly] [NotReplicated] [Deprecated]

## Methods

- **BindToClose**(`function: Function`) -> `null`
- **DefineFastFlag**(`name: string`, `defaultValue: bool`) -> `bool`
- **DefineFastInt**(`name: string`, `defaultValue: int`) -> `int`
- **DefineFastString**(`name: string`, `defaultValue: string`) -> `string`
- **GetEngineFeature**(`name: string`) -> `bool`
- **GetFastFlag**(`name: string`) -> `bool`
- **GetFastInt**(`name: string`) -> `int`
- **GetFastString**(`name: string`) -> `string`
- **GetJobsInfo**() -> `Array`
- **GetMessage**() -> `string` [Deprecated]
- **GetObjects**(`url: ContentId`) -> `Instances`
- **GetObjectsAllOrNone**(`url: ContentId`) -> `Instances`
- **GetObjectsAsync**(`url: ContentId`) -> `Instances` [Yields]
- **GetObjectsList**(`urls: Array`) -> `Array`
- **GetPlaySessionId**() -> `string`
- **GetRemoteBuildMode**() -> `bool` [Deprecated]
- **HttpGetAsync**(`url: string`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **HttpPostAsync**(`url: string`, `data: string`, `contentType: string = */*`, `httpRequestType: HttpRequestType = Default`) -> `string` [Yields]
- **InsertObjectsAndJoinIfLegacyAsync**(`url: ContentId`) -> `Instances` [Yields]
- **IsContentLoaded**() -> `bool`
- **IsGearTypeAllowed**(`gearType: GearType`) -> `bool` [Deprecated]
- **IsLoaded**() -> `bool`
- **IsUniverseMetadataLoaded**() -> `bool`
- **Load**(`url: ContentId`) -> `null`
- **OpenLogsFolder**() -> `null`
- **OpenScreenshotsFolder**() -> `null`
- **OpenVideosFolder**() -> `null`
- **SavePlace**(`saveFilter: SaveFilter = SaveAll`) -> `bool` [Yields] [Deprecated]
- **SetFastFlagForTesting**(`name: string`, `newValue: bool`) -> `bool`
- **SetFastIntForTesting**(`name: string`, `newValue: int`) -> `int`
- **SetFastStringForTesting**(`name: string`, `newValue: string`) -> `string`
- **SetFlagVersion**(`name: string`, `version: int`) -> `null`
- **SetIsLoaded**(`value: bool`, `placeSizeInBytes: int?`) -> `null`
- **SetPlaceId**(`placeId: int64`) -> `null`
- **SetUniverseId**(`universeId: int64`) -> `null`
- **Shutdown**() -> `null`
- **getGameTime**() -> `double`

## Events

- **AllowedGearTypeChanged**() [Deprecated]
- **GraphicsQualityChangeRequest**(`betterQuality: bool`)
- **ItemChanged**(`object: Instance`, `descriptor: string`) [Deprecated]
- **Loaded**()
- **ScreenshotReady**(`path: string`)
- **ScreenshotSavedToAlbum**(`filename: string`, `success: bool`, `message: string`)
- **ServerLifecycleChanged**(`serverLifecycleChangedEvent: Dictionary`)
- **ServerRestartScheduled**(`restartTime: DateTime`, `source: CloseReason`, `attributes: Dictionary`)
- **UniverseMetadataLoaded**()

## Callbacks

- **OnClose**() -> `Tuple` [Deprecated]
