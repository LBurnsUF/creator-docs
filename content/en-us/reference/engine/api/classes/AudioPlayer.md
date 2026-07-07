---
title: AudioPlayer
type: class
superclass: Instance
---

# AudioPlayer

**Inherits from:** `Class.Instance` > `Class.Object`

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.AudioPlayer.Asset` | `Datatype.ContentId` |  |
| `Class.AudioPlayer.AssetId` | `string` | [Hidden] [NotReplicated] [Deprecated] |
| `Class.AudioPlayer.AssetRepresentation` | `Enum.AssetRepresentation` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.AudioPlayer.AudioContent` | `Datatype.Content` | [Hidden] |
| `Class.AudioPlayer.AutoLoad` | `bool` |  |
| `Class.AudioPlayer.AutoPlay` | `bool` |  |
| `Class.AudioPlayer.IsPlaying` | `bool` |  {write: RobloxSecurity} |
| `Class.AudioPlayer.IsReady` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.AudioPlayer.LoopRegion` | `Datatype.NumberRange` |  |
| `Class.AudioPlayer.Looping` | `bool` |  |
| `Class.AudioPlayer.PlaybackRegion` | `Datatype.NumberRange` |  |
| `Class.AudioPlayer.PlaybackSpeed` | `double` |  |
| `Class.AudioPlayer.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.AudioPlayer.TimePosition` | `double` |  |
| `Class.AudioPlayer.Volume` | `float` |  |

## Methods

### `Class.AudioPlayer:Cancel`

``Cancel(actionId: `int64?`)`` → `bool`

### `Class.AudioPlayer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` → `Datatype.Instances`

### `Class.AudioPlayer:GetInputPins`

``GetInputPins()`` → `Array`

### `Class.AudioPlayer:GetOutputPins`

``GetOutputPins()`` → `Array`

### `Class.AudioPlayer:GetWaveformAsync`

``GetWaveformAsync(timeRange: `Datatype.NumberRange`, samples: `int`)`` → `Array`
  [Yields]

### `Class.AudioPlayer:Play`

``Play(atTime: `double?`)`` → `int64?`

### `Class.AudioPlayer:Stop`

``Stop(atTime: `double?`)`` → `int64?`

## Events

### `Class.AudioPlayer.Ended`

Fires with: ()

### `Class.AudioPlayer.Looped`

Fires with: ()

### `Class.AudioPlayer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
