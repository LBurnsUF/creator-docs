---
title: AssetImportService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AssetImportService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetAllPresets**() -> `Dictionary`
- **GetFilesInDirAsync**(`path: string`) -> `Array` [Yields]
- **GetPreset**(`name: string`) -> `Dictionary`
- **PickFileWithPromptAsync**() -> `string` [Yields]
- **PickImageFileWithPrompt**() -> `string` [Yields]
- **PickMeshFileWithPrompt**() -> `string` [Yields]
- **PickMultipleFilesWithPrompt**() -> `Array` [Yields]
- **RemovePreset**(`name: string`) -> `null`
- **SavePreset**(`name: string`, `preset: Dictionary`) -> `bool`
- **StartSessionWithPath**(`filePath: string`) -> `AssetImportSession`
- **StartSessionWithPathAsync**(`filePath: string`) -> `AssetImportSession` [Yields]
- **StartSingleFileWatch**(`filePath: string`) -> `null`
- **StopSingleFileWatch**(`filePath: string`) -> `null`
- **UploadAssetFromContentAsync**(`content: string`, `createAssetRequest: Dictionary`) -> `Tuple` [Yields]
- **UploadAssetFromPathAsync**(`filepath: string`, `createAssetRequest: Dictionary`) -> `Tuple` [Yields]

## Events

- **SingleFileChanged**(`filePath: string`)
- **StartSingleMeshImport**(`fileName: string`)
