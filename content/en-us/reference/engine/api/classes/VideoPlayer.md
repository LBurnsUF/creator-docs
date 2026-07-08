---
title: VideoPlayer
type: class
superclass: Instance
---

# VideoPlayer

Used to play video assets.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

An instance for playing video assets. It can be connected to a
`Class.VideoDisplay` via a `Class.Wire` to show the video and can be connected
to audio instances via a `Class.Wire` to play the audio track.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.VideoPlayer.AutoLoadInStudio` | `bool` | [NotReplicated] [NotScriptable] {write: RobloxScriptSecurity} |
| `Class.VideoPlayer.AutoPlayInStudio` | `bool` | [NotReplicated] [NotScriptable] {write: RobloxScriptSecurity} |
| `Class.VideoPlayer.InternalVideoUsage` | `Enum.InternalVideoUsage` | [Hidden] |
| `Class.VideoPlayer.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.VideoPlayer.IsPlaying` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.VideoPlayer.Looping` | `bool` |  |
| `Class.VideoPlayer.MaximumResolution` | `Enum.VideoSampleSize` | [Hidden] |
| `Class.VideoPlayer.PlaybackSpeed` | `float` |  |
| `Class.VideoPlayer.Resolution` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.VideoPlayer.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.VideoPlayer.TimePosition` | `double` |  |
| `Class.VideoPlayer.VideoContent` | `Datatype.Content` |  |
| `Class.VideoPlayer.Volume` | `float` |  |

## Methods

### `Class.VideoPlayer:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.VideoPlayer:GetInputPins`

``GetInputPins()`` -> `Array`

### `Class.VideoPlayer:GetOutputPins`

``GetOutputPins()`` -> `Array`

### `Class.VideoPlayer:LoadAsync`

``LoadAsync()`` -> `Enum.AssetFetchStatus`
  [Yields]

### `Class.VideoPlayer:Pause`

``Pause()`` -> `null`

### `Class.VideoPlayer:Play`

``Play()`` -> `null`

### `Class.VideoPlayer:SetStudioPreview`

``SetStudioPreview(isPreview: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.VideoPlayer:Unload`

``Unload()`` -> `null`

## Events

### `Class.VideoPlayer.DidEnd`

Fires with: ()

### `Class.VideoPlayer.DidLoop`

Fires with: ()

### `Class.VideoPlayer.PlayFailed`

Fires with: (error: `Enum.AssetFetchStatus`)

### `Class.VideoPlayer.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
