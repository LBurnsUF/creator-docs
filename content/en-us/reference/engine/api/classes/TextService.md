---
title: TextService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# TextService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **FilterAndTranslateStringAsync**(`stringToFilter: string`, `fromUserId: int64`, `targetLocales: Array`, `textContext: TextFilterContext = PrivateChat`) -> `TextFilterTranslatedResult` [Yields]
- **FilterStringAsync**(`stringToFilter: string`, `fromUserId: int64`, `textContext: TextFilterContext = PrivateChat`) -> `TextFilterResult` [Yields]
- **GetFamilyInfoAsync**(`assetId: ContentId`) -> `Dictionary` [Yields]
- **GetFontMemoryData**() -> `Dictionary`
- **GetTextBoundsAsync**(`params: GetTextBoundsParams`) -> `Vector2` [Yields]
- **GetTextSize**(`string: string`, `fontSize: int`, `font: Font`, `frameSize: Vector2`) -> `Vector2`
- **GetTextSizeOffsetAsync**(`fontSize: int`, `font: Font`) -> `float` [Yields]
- **SetResolutionScale**(`scale: float`) -> `null`
