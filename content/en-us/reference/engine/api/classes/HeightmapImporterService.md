---
title: HeightmapImporterService
type: class
superclass: Instance
tags: [Service, NotReplicated]
---

# HeightmapImporterService

**Inherits**: Instance > Object

**Tags**: Service, NotReplicated

## Methods

- **CancelImportHeightmap**() -> `null`
- **GetHeightmapPreviewAsync**(`heightmapAssetId: ContentId`) -> `Tuple` [Yields]
- **ImportHeightmap**(`region: Region3`, `heightmapAssetId: ContentId`, `colormapAssetId: ContentId`, `defaultMaterial: Material`) -> `null` [Yields]
- **IsValidColormap**(`colormapAssetId: ContentId`) -> `Tuple`
- **IsValidHeightmap**(`heightmapAssetId: ContentId`) -> `Tuple`
- **SetImportHeightmapPaused**(`paused: bool`) -> `null`

## Events

- **ColormapHasUnknownPixels**()
- **ProgressUpdate**(`progressRatio: float`, `operation: string`)
