---
title: StudioService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **ActiveScript**: `Instance` [ReadOnly] [NotReplicated]
- **AlignDraggedObjects**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **DraggerSolveConstraints**: `bool` [ReadOnly] [NotReplicated]
- **DrawConstraintsOnTop**: `bool` [ReadOnly] [NotReplicated] [Deprecated]
- **GridSize**: `float` [ReadOnly] [NotReplicated]
- **HoverInstance**: `Instance` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **InstalledPluginData**: `string` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PivotSnapToGeometry**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RotateIncrement**: `float` [ReadOnly] [NotReplicated]
- **Secrets**: `string` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ShowConstraintDetails**: `bool` [ReadOnly] [NotReplicated]
- **ShowWeldDetails**: `bool` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **StudioLocaleId**: `string` [ReadOnly] [NotReplicated]
- **UseLocalSpace**: `bool` [NotReplicated]

## Methods

- **AnimationIdSelected**(`id: int64`) -> `null`
- **CopyToClipboard**(`stringToCopy: string`) -> `null`
- **GetBadgeConfigureUrl**(`badgeId: int64`) -> `string`
- **GetBadgeUploadUrl**() -> `string`
- **GetClassIcon**(`className: string`) -> `Dictionary`
- **GetPlaceIsPersistedToCloud**() -> `bool`
- **GetResourceByCategory**(`category: string`) -> `Dictionary`
- **GetStartupAssetId**() -> `string`
- **GetStartupPluginId**() -> `string`
- **GetTermsOfUseUrl**() -> `string`
- **GetUserId**() -> `int64`
- **GizmoRaycast**(`origin: Vector3`, `direction: Vector3`, `raycastParams: RaycastParams = RaycastParams{IgnoreWater=false, BruteForceAllSlow=false, RespectCanCollide=false, CollisionGroup=Default, FilterDescendantsInstances={}}`) -> `RaycastResult?`
- **HasInternalPermission**() -> `bool`
- **IsPluginInstalled**(`assetId: int64`) -> `bool`
- **IsPluginUpToDate**(`assetId: int64`, `currentAssetVersion: int64`) -> `bool`
- **OpenInBrowser_DONOTUSE**(`url: string`) -> `null`
- **PromptImportFile**(`fileTypeFilter: Array = {}`) -> `Instance` [Yields] [Deprecated]
- **PromptImportFileAsync**(`fileTypeFilter: Array = {}`) -> `Instance` [Yields]
- **PromptImportFiles**(`fileTypeFilter: Array = {}`) -> `Instances` [Yields] [Deprecated]
- **PromptImportFilesAsync**(`fileTypeFilter: Array = {}`) -> `Instances` [Yields]
- **SetPluginEnabled**(`assetId: int64`, `state: bool`) -> `null`
- **ShowPublishToRoblox**() -> `null`
- **TryInstallPlugin**(`assetId: int64`, `assetVersionId: int64`) -> `null` [Yields]
- **UninstallPlugin**(`assetId: int64`) -> `null`
- **UpdatePluginManagement**() -> `null`

## Events

- **OnImportFromRoblox**(`assetType: string`)
- **OnOpenGameSettings**(`pageIdentifier: string`)
- **OnOpenManagePackagePlugin**(`userId: int64`, `assetId: int64`)
- **OnPluginInstalledFromToolbox**()
- **OnPluginInstalledFromWeb**(`pluginId: string`)
- **OnPublishAsPlugin**(`instances: Instances`)
- **OnSaveToRoblox**(`instances: Instances`)
- **PromptTransformPluginCheckEnable**()
- **SaveLocallyAsComplete**(`success: bool`)
