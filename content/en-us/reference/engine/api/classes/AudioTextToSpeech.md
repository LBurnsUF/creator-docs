---
title: AudioTextToSpeech
type: class
superclass: Instance
---

# AudioTextToSpeech

Plays text as speech audio.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioTextToSpeech` is used to play text as speech audio. It provides a
single **Output** pin which can be connected to other pins via
`Class.Wire|Wires`.

Roblox uses the following formula to throttle requests for this API based on
the number of players in your experience:
`max requests per minute per experience = 1 + (6 * number_of_concurrent_users)`.
You can purchase additional usage using
[Extended Services](../../../cloud-services/extended-services.md).

For a more in-depth look, see
[Text-to-speech](../../../audio/objects.md#text-to-speech).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioTextToSpeech.IsLoaded` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.AudioTextToSpeech.IsPlaying` | `bool` |  {write: RobloxSecurity} |
| `Class.AudioTextToSpeech.Looping` | `bool` |  |
| `Class.AudioTextToSpeech.Pitch` | `float` |  |
| `Class.AudioTextToSpeech.PlaybackSpeed` | `float` |  |
| `Class.AudioTextToSpeech.Speed` | `float` |  |
| `Class.AudioTextToSpeech.Text` | `string` |  |
| `Class.AudioTextToSpeech.TimeLength` | `double` | [ReadOnly] [NotReplicated] |
| `Class.AudioTextToSpeech.TimePosition` | `double` |  |
| `Class.AudioTextToSpeech.VoiceId` | `string` |  |
| `Class.AudioTextToSpeech.Volume` | `float` |  |

## Methods

### `Class.AudioTextToSpeech:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

### `Class.AudioTextToSpeech:GetWaveformAsync`

``GetWaveformAsync(timeRange: `Datatype.NumberRange`, samples: `int`)`` -> `Array`
  [Yields]

### `Class.AudioTextToSpeech:LoadAsync`

``LoadAsync()`` -> `Enum.AssetFetchStatus`
  [Yields]

### `Class.AudioTextToSpeech:Pause`

``Pause()`` -> `null`

### `Class.AudioTextToSpeech:Play`

``Play()`` -> `null`

### `Class.AudioTextToSpeech:Unload`

``Unload()`` -> `null`

## Events

### `Class.AudioTextToSpeech.Ended`

Fires with: ()

### `Class.AudioTextToSpeech.Looped`

Fires with: ()

### `Class.AudioTextToSpeech.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
