---
title: StudioService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.StudioService.ActiveScript` | `Class.Instance` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.AlignDraggedObjects` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioService.DraggerSolveConstraints` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.DrawConstraintsOnTop` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.StudioService.GridSize` | `float` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.HoverInstance` | `Class.Instance` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioService.InstalledPluginData` | `string` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioService.PivotSnapToGeometry` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioService.RotateIncrement` | `float` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.Secrets` | `string` |  {security: RobloxScriptSecurity} |
| `Class.StudioService.ShowConstraintDetails` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.ShowWeldDetails` | `bool` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioService.StudioLocaleId` | `string` | [ReadOnly] [NotReplicated] |
| `Class.StudioService.UseLocalSpace` | `bool` | [NotReplicated] |

## Methods

### `Class.StudioService:AnimationIdSelected`

``AnimationIdSelected(id: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:CopyToClipboard`

``CopyToClipboard(stringToCopy: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetBadgeConfigureUrl`

``GetBadgeConfigureUrl(badgeId: `int64`)`` → `string`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetBadgeUploadUrl`

``GetBadgeUploadUrl()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetClassIcon`

``GetClassIcon(className: `string`)`` → `Dictionary`
   {security: PluginSecurity}

### `Class.StudioService:GetPlaceIsPersistedToCloud`

``GetPlaceIsPersistedToCloud()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetResourceByCategory`

``GetResourceByCategory(category: `string`)`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetStartupAssetId`

``GetStartupAssetId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetStartupPluginId`

``GetStartupPluginId()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetTermsOfUseUrl`

``GetTermsOfUseUrl()`` → `string`
   {security: RobloxScriptSecurity}

### `Class.StudioService:GetUserId`

``GetUserId()`` → `int64`
   {security: PluginSecurity}

### `Class.StudioService:GizmoRaycast`

``GizmoRaycast(origin: `Datatype.Vector3`, direction: `Datatype.Vector3`, raycastParams: `Datatype.RaycastParams`)`` → `Datatype.RaycastResult`?
   {security: PluginSecurity}

### `Class.StudioService:HasInternalPermission`

``HasInternalPermission()`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.StudioService:IsPluginInstalled`

``IsPluginInstalled(assetId: `int64`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.StudioService:IsPluginUpToDate`

``IsPluginUpToDate(assetId: `int64`, currentAssetVersion: `int64`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.StudioService:OpenInBrowser_DONOTUSE`

``OpenInBrowser_DONOTUSE(url: `string`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:PromptImportFile`

``PromptImportFile(fileTypeFilter: `Array`)`` → `Class.Instance`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.StudioService:PromptImportFileAsync`

``PromptImportFileAsync(fileTypeFilter: `Array`)`` → `Class.Instance`
  [Yields] {security: PluginSecurity}

### `Class.StudioService:PromptImportFiles`

``PromptImportFiles(fileTypeFilter: `Array`)`` → `Datatype.Instances`
  [Yields] [Deprecated] {security: PluginSecurity}

### `Class.StudioService:PromptImportFilesAsync`

``PromptImportFilesAsync(fileTypeFilter: `Array`)`` → `Datatype.Instances`
  [Yields] {security: PluginSecurity}

### `Class.StudioService:SetPluginEnabled`

``SetPluginEnabled(assetId: `int64`, state: `bool`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:ShowPublishToRoblox`

``ShowPublishToRoblox()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:TryInstallPlugin`

``TryInstallPlugin(assetId: `int64`, assetVersionId: `int64`)`` → `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioService:UninstallPlugin`

``UninstallPlugin(assetId: `int64`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.StudioService:UpdatePluginManagement`

``UpdatePluginManagement()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.StudioService.OnImportFromRoblox`

Fires with: (assetType: `string`)

### `Class.StudioService.OnOpenGameSettings`

Fires with: (pageIdentifier: `string`)

### `Class.StudioService.OnOpenManagePackagePlugin`

Fires with: (userId: `int64`, assetId: `int64`)

### `Class.StudioService.OnPluginInstalledFromToolbox`

Fires with: ()

### `Class.StudioService.OnPluginInstalledFromWeb`

Fires with: (pluginId: `string`)

### `Class.StudioService.OnPublishAsPlugin`

Fires with: (instances: `Datatype.Instances`)

### `Class.StudioService.OnSaveToRoblox`

Fires with: (instances: `Datatype.Instances`)

### `Class.StudioService.PromptTransformPluginCheckEnable`

Fires with: ()

### `Class.StudioService.SaveLocallyAsComplete`

Fires with: (success: `bool`)
