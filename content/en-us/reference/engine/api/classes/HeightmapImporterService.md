---
title: HeightmapImporterService
type: class
superclass: Instance
tags: [Service, NotReplicated]
---

# HeightmapImporterService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [Service] [NotReplicated]

## Methods

### `Class.HeightmapImporterService:CancelImportHeightmap`

``CancelImportHeightmap()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.HeightmapImporterService:GetHeightmapPreviewAsync`

``GetHeightmapPreviewAsync(heightmapAssetId: `Datatype.ContentId`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HeightmapImporterService:ImportHeightmap`

``ImportHeightmap(region: `Datatype.Region3`, heightmapAssetId: `Datatype.ContentId`, colormapAssetId: `Datatype.ContentId`, defaultMaterial: `Enum.Material`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.HeightmapImporterService:IsValidColormap`

``IsValidColormap(colormapAssetId: `Datatype.ContentId`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.HeightmapImporterService:IsValidHeightmap`

``IsValidHeightmap(heightmapAssetId: `Datatype.ContentId`)`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.HeightmapImporterService:SetImportHeightmapPaused`

``SetImportHeightmapPaused(paused: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.HeightmapImporterService.ColormapHasUnknownPixels`

Fires with: ()

### `Class.HeightmapImporterService.ProgressUpdate`

Fires with: (progressRatio: `float`, operation: `string`)
