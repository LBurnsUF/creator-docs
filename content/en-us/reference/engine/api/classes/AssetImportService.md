---
title: AssetImportService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetImportService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AssetImportService:GetAllPresets`

``GetAllPresets()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:GetFilesInDirAsync`

``GetFilesInDirAsync(path: `string`)`` -> `Array`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:GetPreset`

``GetPreset(name: `string`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:PickFileWithPromptAsync`

``PickFileWithPromptAsync()`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:PickImageFileWithPrompt`

``PickImageFileWithPrompt()`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:PickMeshFileWithPrompt`

``PickMeshFileWithPrompt()`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:PickMultipleFilesWithPrompt`

``PickMultipleFilesWithPrompt()`` -> `Array`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:RemovePreset`

``RemovePreset(name: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:SavePreset`

``SavePreset(name: `string`, preset: `Dictionary`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:StartSessionWithPath`

``StartSessionWithPath(filePath: `string`)`` -> `Class.AssetImportSession`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:StartSessionWithPathAsync`

``StartSessionWithPathAsync(filePath: `string`)`` -> `Class.AssetImportSession`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:StartSingleFileWatch`

``StartSingleFileWatch(filePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:StopSingleFileWatch`

``StopSingleFileWatch(filePath: `string`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AssetImportService:UploadAssetFromContentAsync`

``UploadAssetFromContentAsync(content: `string`, createAssetRequest: `Dictionary`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

### `Class.AssetImportService:UploadAssetFromPathAsync`

``UploadAssetFromPathAsync(filepath: `string`, createAssetRequest: `Dictionary`)`` -> `Tuple`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.AssetImportService.SingleFileChanged`

Fires with: (filePath: `string`)

### `Class.AssetImportService.StartSingleMeshImport`

Fires with: (fileName: `string`)
