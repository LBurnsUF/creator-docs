---
title: Sound
type: class
superclass: Instance
---

# Sound

An object that emits sound. This object can be placed within a
`Class.BasePart` or `Class.Attachment` to emit a sound from a particular
position within a place or world, or it can be attached elsewhere to play the
sound at a constant volume throughout the entire place.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.Sound` is an object that emits sound. When placed in a `Class.BasePart`
or an `Class.Attachment`, this object will emit its sound from that part's
`Class.BasePart.Position` or the attachment's
`Class.Attachment.WorldPosition`. In this placement, a `Class.Sound` exhibits
the Doppler effect, meaning its frequency and pitch varies with the relative
motion of whatever attachment or part it is attached to. Additionally, its
volume will be determined by the distance between the client's sound listener
(by default the `Class.Camera` position) and the position of the sound's
parent. For more information, see `Class.Sound.RollOffMode|RollOffMode`.

A sound is considered "global" if it is **not** parented to a `Class.BasePart`
or an `Class.Attachment`. In this case, the sound will play at the same volume
throughout the entire place.

## Properties

| Property | Type | Description |
|----------|------|-------------|
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

``GetUnderlyingAudioPlayer()`` -> `Class.AudioPlayer`
   {security: RobloxScriptSecurity}

### `Class.Sound:Pause`

``Pause()`` -> `null`

### `Class.Sound:Play`

``Play()`` -> `null`

### `Class.Sound:Resume`

``Resume()`` -> `null`

### `Class.Sound:Stop`

``Stop()`` -> `null`

### `Class.Sound:pause`

``pause()`` -> `null`
  [Deprecated]

### `Class.Sound:play`

``play()`` -> `null`
  [Deprecated]

### `Class.Sound:stop`

``stop()`` -> `null`
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
