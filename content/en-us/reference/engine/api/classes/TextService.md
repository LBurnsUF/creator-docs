---
title: TextService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# TextService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.TextService:FilterAndTranslateStringAsync`

``FilterAndTranslateStringAsync(stringToFilter: `string`, fromUserId: `int64`, targetLocales: `Array`, textContext: `Enum.TextFilterContext`)`` → `Class.TextFilterTranslatedResult`
  [Yields]

### `Class.TextService:FilterStringAsync`

``FilterStringAsync(stringToFilter: `string`, fromUserId: `int64`, textContext: `Enum.TextFilterContext`)`` → `Class.TextFilterResult`
  [Yields]

### `Class.TextService:GetFamilyInfoAsync`

``GetFamilyInfoAsync(assetId: `Datatype.ContentId`)`` → `Dictionary`
  [Yields]

### `Class.TextService:GetFontMemoryData`

``GetFontMemoryData()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.TextService:GetTextBoundsAsync`

``GetTextBoundsAsync(params: `Class.GetTextBoundsParams`)`` → `Datatype.Vector2`
  [Yields]

### `Class.TextService:GetTextSize`

``GetTextSize(string: `string`, fontSize: `int`, font: `Enum.Font`, frameSize: `Datatype.Vector2`)`` → `Datatype.Vector2`

### `Class.TextService:GetTextSizeOffsetAsync`

``GetTextSizeOffsetAsync(fontSize: `int`, font: `Datatype.Font`)`` → `float`
  [Yields]

### `Class.TextService:SetResolutionScale`

``SetResolutionScale(scale: `float`)`` → `null`
   {security: RobloxScriptSecurity}
