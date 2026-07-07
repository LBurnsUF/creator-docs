---
title: Sound
type: class
superclass: Instance
---

# Sound

**Inherits**: Instance > Object

## Properties

- **AcousticSimulationEnabled**: `bool`
- **AssetRepresentation**: `AssetRepresentation` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **AudioContent**: `Content` [Hidden]
- **ChannelCount**: `int` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **EmitterSize**: `float` [Deprecated]
- **IsLoaded**: `bool` [ReadOnly] [NotReplicated]
- **IsPaused**: `bool` [Hidden] [ReadOnly] [NotReplicated]
- **IsPlaying**: `bool` [Hidden] [ReadOnly] [NotReplicated]
- **IsSpatial**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LoopRegion**: `NumberRange`
- **Looped**: `bool`
- **MaxDistance**: `float` [Deprecated]
- **MinDistance**: `float` [Deprecated]
- **Pitch**: `float` [Deprecated]
- **PlayOnRemove**: `bool`
- **PlaybackLoudness**: `double` [ReadOnly] [NotReplicated]
- **PlaybackRegion**: `NumberRange`
- **PlaybackRegionsEnabled**: `bool`
- **PlaybackSpeed**: `float` [NotReplicated]
- **Playing**: `bool` [NotReplicated]
- **RollOffGain**: `float` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **RollOffMaxDistance**: `float`
- **RollOffMinDistance**: `float`
- **RollOffMode**: `RollOffMode`
- **SoundGroup**: `SoundGroup`
- **SoundId**: `ContentId`
- **TimeLength**: `double` [ReadOnly] [NotReplicated]
- **TimePosition**: `double` [NotReplicated]
- **UsageContextPermission**: `UsageContext` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Volume**: `float`
- **isPlaying**: `bool` [ReadOnly] [NotReplicated] [Deprecated]

## Methods

- **GetUnderlyingAudioPlayer**() -> `AudioPlayer`
- **Pause**() -> `null`
- **Play**() -> `null`
- **Resume**() -> `null`
- **Stop**() -> `null`
- **pause**() -> `null` [Deprecated]
- **play**() -> `null` [Deprecated]
- **stop**() -> `null` [Deprecated]

## Events

- **DidLoop**(`soundId: string`, `numOfTimesLooped: int`)
- **Ended**(`soundId: string`)
- **Loaded**(`soundId: string`)
- **Paused**(`soundId: string`)
- **Played**(`soundId: string`)
- **Resumed**(`soundId: string`)
- **Stopped**(`soundId: string`)
