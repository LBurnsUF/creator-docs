---
title: VideoPlayer
type: class
superclass: Instance
---

# VideoPlayer

**Inherits**: Instance > Object

## Properties

- **AutoLoadInStudio**: `bool` [NotReplicated] [NotScriptable] (Security: Read=None, Write=RobloxScriptSecurity)
- **AutoPlayInStudio**: `bool` [NotReplicated] [NotScriptable] (Security: Read=None, Write=RobloxScriptSecurity)
- **InternalVideoUsage**: `InternalVideoUsage` [Hidden]
- **IsLoaded**: `bool` [ReadOnly] [NotReplicated]
- **IsPlaying**: `bool` [ReadOnly] [NotReplicated]
- **Looping**: `bool`
- **MaximumResolution**: `VideoSampleSize` [Hidden]
- **PlaybackSpeed**: `float`
- **Resolution**: `Vector2` [ReadOnly] [NotReplicated]
- **TimeLength**: `double` [ReadOnly] [NotReplicated]
- **TimePosition**: `double`
- **VideoContent**: `Content`
- **Volume**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **LoadAsync**() -> `AssetFetchStatus` [Yields]
- **Pause**() -> `null`
- **Play**() -> `null`
- **SetStudioPreview**(`isPreview: bool`) -> `null`
- **Unload**() -> `null`

## Events

- **DidEnd**()
- **DidLoop**()
- **PlayFailed**(`error: AssetFetchStatus`)
- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)
