---
title: VideoFrame
type: class
superclass: GuiObject
---

# VideoFrame

**Inherits**: GuiObject > GuiBase2d > GuiBase > Instance > Object

## Properties

- **InternalVideoUsage**: `InternalVideoUsage` [Hidden]
- **IsLoaded**: `bool` [ReadOnly] [NotReplicated]
- **Looped**: `bool`
- **MaximumResolution**: `VideoSampleSize` [Hidden]
- **Playing**: `bool` [NotReplicated]
- **Resolution**: `Vector2` [ReadOnly] [NotReplicated]
- **RollOffMaxDistance**: `float`
- **RollOffMinDistance**: `float`
- **RollOffMode**: `RollOffMode`
- **TimeLength**: `double` [ReadOnly] [NotReplicated]
- **TimePosition**: `double` [NotReplicated]
- **Video**: `ContentId`
- **VideoContent**: `Content`
- **Volume**: `float`

## Methods

- **Pause**() -> `null`
- **Play**() -> `null`
- **SetStudioPreview**(`isPreview: bool`) -> `null`

## Events

- **DidLoop**(`video: string`)
- **Ended**(`video: string`)
- **Loaded**(`video: string`)
- **Paused**(`video: string`)
- **Played**(`video: string`)
