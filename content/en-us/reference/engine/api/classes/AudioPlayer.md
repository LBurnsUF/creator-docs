---
title: AudioPlayer
type: class
superclass: Instance
---

# AudioPlayer

**Inherits**: Instance > Object

## Properties

- **Asset**: `ContentId`
- **AssetId**: `string` [Hidden] [NotReplicated] [Deprecated]
- **AssetRepresentation**: `AssetRepresentation` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **AudioContent**: `Content` [Hidden]
- **AutoLoad**: `bool`
- **AutoPlay**: `bool`
- **IsPlaying**: `bool` (Security: Read=None, Write=RobloxSecurity)
- **IsReady**: `bool` [ReadOnly] [NotReplicated]
- **LoopRegion**: `NumberRange`
- **Looping**: `bool`
- **PlaybackRegion**: `NumberRange`
- **PlaybackSpeed**: `double`
- **TimeLength**: `double` [ReadOnly] [NotReplicated]
- **TimePosition**: `double`
- **Volume**: `float`

## Methods

- **Cancel**(`actionId: int64?`) -> `bool`
- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetInputPins**() -> `Array`
- **GetOutputPins**() -> `Array`
- **GetWaveformAsync**(`timeRange: NumberRange`, `samples: int`) -> `Array` [Yields]
- **Play**(`atTime: double?`) -> `int64?`
- **Stop**(`atTime: double?`) -> `int64?`

## Events

- **Ended**()
- **Looped**()
- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)
