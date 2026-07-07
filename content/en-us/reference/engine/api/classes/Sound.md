---
title: Sound
type: class
superclass: Instance
---

# Sound

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.Sound.AcousticSimulationEnabled` | `bool` |  |
| `Class.Sound.AssetRepresentation` | `Enum.AssetRepresentation` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Sound.AudioContent` | `Datatype.Content` | [Hidden] |
| `Class.Sound.ChannelCount` | `int` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Sound.EmitterSize` | `float` | [Deprecated] |
| `Class.Sound.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Sound.IsPaused` | `bool` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.Sound.IsPlaying` | `bool` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.Sound.IsSpatial` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Sound.LoopRegion` | `Datatype.NumberRange` |  |
| `Class.Sound.Looped` | `bool` |  |
| `Class.Sound.MaxDistance` | `float` | [Deprecated] |
| `Class.Sound.MinDistance` | `float` | [Deprecated] |
| `Class.Sound.Pitch` | `float` | [Deprecated] |
| `Class.Sound.PlayOnRemove` | `bool` |  |
| `Class.Sound.PlaybackLoudness` | `double` | [ReadOnly] [NotReplicated] |
| `Class.Sound.PlaybackRegion` | `Datatype.NumberRange` |  |
| `Class.Sound.PlaybackRegionsEnabled` | `bool` |  |
| `Class.Sound.PlaybackSpeed` | `float` | [NotReplicated] |
| `Class.Sound.Playing` | `bool` | [NotReplicated] |
| `Class.Sound.RollOffGain` | `float` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Sound.RollOffMaxDistance` | `float` |  |
| `Class.Sound.RollOffMinDistance` | `float` |  |
| `Class.Sound.RollOffMode` | `Enum.RollOffMode` |  |
| `Class.Sound.SoundGroup` | `Class.SoundGroup` |  |
| `Class.Sound.SoundId` | `Datatype.ContentId` |  |
| `Class.Sound.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.Sound.TimePosition` | `double` | [NotReplicated] |
| `Class.Sound.UsageContextPermission` | `Enum.UsageContext` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.Sound.Volume` | `float` |  |
| `Class.Sound.isPlaying` | `bool` | [ReadOnly] [NotReplicated] [Deprecated] |

## Methods

### `Class.Sound:GetUnderlyingAudioPlayer`

``GetUnderlyingAudioPlayer()`` → `Class.AudioPlayer`
   {security: RobloxScriptSecurity}

### `Class.Sound:Pause`

``Pause()`` → `null`

### `Class.Sound:Play`

``Play()`` → `null`

### `Class.Sound:Resume`

``Resume()`` → `null`

### `Class.Sound:Stop`

``Stop()`` → `null`

### `Class.Sound:pause`

``pause()`` → `null`
  [Deprecated]

### `Class.Sound:play`

``play()`` → `null`
  [Deprecated]

### `Class.Sound:stop`

``stop()`` → `null`
  [Deprecated]

## Events

### `Class.Sound.DidLoop`

Fires with: (soundId: `string`, numOfTimesLooped: `int`)

### `Class.Sound.Ended`

Fires with: (soundId: `string`)

### `Class.Sound.Loaded`

Fires with: (soundId: `string`)

### `Class.Sound.Paused`

Fires with: (soundId: `string`)

### `Class.Sound.Played`

Fires with: (soundId: `string`)

### `Class.Sound.Resumed`

Fires with: (soundId: `string`)

### `Class.Sound.Stopped`

Fires with: (soundId: `string`)
