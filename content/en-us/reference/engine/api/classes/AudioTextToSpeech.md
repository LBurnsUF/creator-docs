---
title: AudioTextToSpeech
type: class
superclass: Instance
---

# AudioTextToSpeech

**Inherits**: Instance > Object

## Properties

- **IsLoaded**: `bool` [ReadOnly] [NotReplicated]
- **IsPlaying**: `bool` (Security: Read=None, Write=RobloxSecurity)
- **Looping**: `bool`
- **Pitch**: `float`
- **PlaybackSpeed**: `float`
- **Speed**: `float`
- **Text**: `string`
- **TimeLength**: `double` [ReadOnly] [NotReplicated]
- **TimePosition**: `double`
- **VoiceId**: `string`
- **Volume**: `float`

## Methods

- **GetConnectedWires**(`pin: string`) -> `Instances`
- **GetWaveformAsync**(`timeRange: NumberRange`, `samples: int`) -> `Array` [Yields]
- **LoadAsync**() -> `AssetFetchStatus` [Yields]
- **Pause**() -> `null`
- **Play**() -> `null`
- **Unload**() -> `null`

## Events

- **Ended**()
- **Looped**()
- **WiringChanged**(`connected: bool`, `pin: string`, `wire: Wire`, `instance: Instance`)
