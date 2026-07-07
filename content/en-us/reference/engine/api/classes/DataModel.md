---
title: DataModel
type: class
superclass: ServiceProvider
tags: [NotCreatable]
---

# DataModel

**Inherits from:** `Class.ServiceProvider` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.DataModel.CreatorId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.CreatorType` | `Enum.CreatorType` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.Environment` | `string` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.DataModel.GameId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.GearGenreSetting` | `Enum.GearGenreSetting` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.DataModel.Genre` | `Enum.Genre` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.IsSFFlagsLoaded` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.DataModel.JobId` | `string` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.MatchmakingType` | `Enum.MatchmakingType` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.PlaceId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.PlaceVersion` | `int` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.PrivateServerId` | `string` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.PrivateServerOwnerId` | `int64` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.RunService` | `Class.RunService` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.VIPServerId` | `string` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.DataModel.VIPServerOwnerId` | `int64` | [Hidden] [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.DataModel.Workspace` | `Class.Workspace` | [ReadOnly] [NotReplicated] |
| `Class.DataModel.lighting` | `Class.Instance` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.DataModel.workspace` | `Class.Workspace` | [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.DataModel:BindToClose`

``BindToClose(function: `Datatype.Function`)`` → `null`

### `Class.DataModel:DefineFastFlag`

``DefineFastFlag(name: `string`, defaultValue: `bool`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.DataModel:DefineFastInt`

``DefineFastInt(name: `string`, defaultValue: `int`)`` → `int`
   {security: RobloxScriptSecurity}

### `Class.DataModel:DefineFastString`

``DefineFastString(name: `string`, defaultValue: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.DataModel:GetEngineFeature`

``GetEngineFeature(name: `string`)`` → `bool`
   {security: LocalUserSecurity}

### `Class.DataModel:GetFastFlag`

``GetFastFlag(name: `string`)`` → `bool`
   {security: LocalUserSecurity}

### `Class.DataModel:GetFastInt`

``GetFastInt(name: `string`)`` → `int`
   {security: LocalUserSecurity}

### `Class.DataModel:GetFastString`

``GetFastString(name: `string`)`` → `string`
   {security: LocalUserSecurity}

### `Class.DataModel:GetJobsInfo`

``GetJobsInfo()`` → `Array`
   {security: PluginSecurity}

### `Class.DataModel:GetMessage`

``GetMessage()`` → `string`
  [Deprecated]

### `Class.DataModel:GetObjects`

``GetObjects(url: `Datatype.ContentId`)`` → `Datatype.Instances`
   {security: PluginSecurity}

### `Class.DataModel:GetObjectsAllOrNone`

``GetObjectsAllOrNone(url: `Datatype.ContentId`)`` → `Datatype.Instances`
   {security: RobloxScriptSecurity}

### `Class.DataModel:GetObjectsAsync`

``GetObjectsAsync(url: `Datatype.ContentId`)`` → `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DataModel:GetObjectsList`

``GetObjectsList(urls: `Array`)`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.DataModel:GetPlaySessionId`

``GetPlaySessionId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.DataModel:GetRemoteBuildMode`

``GetRemoteBuildMode()`` → `bool`
  [Deprecated]

### `Class.DataModel:HttpGetAsync`

``HttpGetAsync(url: `string`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DataModel:HttpPostAsync`

``HttpPostAsync(url: `string`, data: `string`, contentType: `string`, httpRequestType: `Enum.HttpRequestType`)`` → `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DataModel:InsertObjectsAndJoinIfLegacyAsync`

``InsertObjectsAndJoinIfLegacyAsync(url: `Datatype.ContentId`)`` → `Datatype.Instances`
  [Yields] {security: RobloxScriptSecurity}

### `Class.DataModel:IsContentLoaded`

``IsContentLoaded()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.DataModel:IsGearTypeAllowed`

``IsGearTypeAllowed(gearType: `Enum.GearType`)`` → `bool`
  [Deprecated]

### `Class.DataModel:IsLoaded`

``IsLoaded()`` → `bool`

### `Class.DataModel:IsUniverseMetadataLoaded`

``IsUniverseMetadataLoaded()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.DataModel:Load`

``Load(url: `Datatype.ContentId`)`` → `null`
   {security: LocalUserSecurity}

### `Class.DataModel:OpenLogsFolder`

``OpenLogsFolder()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModel:OpenScreenshotsFolder`

``OpenScreenshotsFolder()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModel:OpenVideosFolder`

``OpenVideosFolder()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SavePlace`

``SavePlace(saveFilter: `Enum.SaveFilter`)`` → `bool`
  [Yields] [Deprecated]

### `Class.DataModel:SetFastFlagForTesting`

``SetFastFlagForTesting(name: `string`, newValue: `bool`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SetFastIntForTesting`

``SetFastIntForTesting(name: `string`, newValue: `int`)`` → `int`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SetFastStringForTesting`

``SetFastStringForTesting(name: `string`, newValue: `string`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SetFlagVersion`

``SetFlagVersion(name: `string`, version: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SetIsLoaded`

``SetIsLoaded(value: `bool`, placeSizeInBytes: `int?`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.DataModel:SetPlaceId`

``SetPlaceId(placeId: `int64`)`` → `null`
   {security: PluginSecurity}

### `Class.DataModel:SetUniverseId`

``SetUniverseId(universeId: `int64`)`` → `null`
   {security: PluginSecurity}

### `Class.DataModel:Shutdown`

``Shutdown()`` → `null`
   {security: LocalUserSecurity}

### `Class.DataModel:getGameTime`

``getGameTime()`` → `double`
   {security: RobloxScriptSecurity}

## Events

### `Class.DataModel.AllowedGearTypeChanged`

Fires with: ()
  [Deprecated]

### `Class.DataModel.GraphicsQualityChangeRequest`

Fires with: (betterQuality: `bool`)

### `Class.DataModel.ItemChanged`

Fires with: (object: `Class.Instance`, descriptor: `string`)
  [Deprecated]

### `Class.DataModel.Loaded`

Fires with: ()

### `Class.DataModel.ScreenshotReady`

Fires with: (path: `string`)

### `Class.DataModel.ScreenshotSavedToAlbum`

Fires with: (filename: `string`, success: `bool`, message: `string`)

### `Class.DataModel.ServerLifecycleChanged`

Fires with: (serverLifecycleChangedEvent: `Dictionary`)

### `Class.DataModel.ServerRestartScheduled`

Fires with: (restartTime: `Datatype.DateTime`, source: `Enum.CloseReason`, attributes: `Dictionary`)

### `Class.DataModel.UniverseMetadataLoaded`

Fires with: ()

## Callbacks

### `Class.DataModel.OnClose`

``OnClose()`` → `Tuple`
  [Deprecated]
