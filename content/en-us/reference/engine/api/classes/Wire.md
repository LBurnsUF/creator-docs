---
title: Wire
type: class
superclass: Instance
---

# Wire

Connects one or more `Class.Instance|Instances` to form a processing graph of
their streams. At the moment, only audio streams are supported, but this may
expand in the future.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.Wire` connects one or more `Class.Instance|Instances` to form a
processing graph of their streams. Each `Class.Wire` connects a source and
target instance, and a source and target "pin" within each of those instances.
Pins are string identifiers that select which stream is to be carried by the
wire.

At the moment, only audio streams are supported, but this may expand in the
future.

The following instances may be connected by `Class.Wire|Wires`:

- `Class.AudioAnalyzer`
- `Class.AudioChannelMixer`
- `Class.AudioChannelSplitter`
- `Class.AudioChorus`
- `Class.AudioCompressor`
- `Class.AudioDeviceInput`
- `Class.AudioDeviceOutput`
- `Class.AudioDistortion`
- `Class.AudioEcho`
- `Class.AudioEmitter`
- `Class.AudioEqualizer`
- `Class.AudioFader`
- `Class.AudioFilter`
- `Class.AudioFlanger`
- `Class.AudioGate`
- `Class.AudioLimiter`
- `Class.AudioListener`
- `Class.AudioPitchShifter`
- `Class.AudioPlayer`
- `Class.AudioRecorder`
- `Class.AudioReverb`
- `Class.AudioSpeechToText`
- `Class.AudioTextToSpeech`
- `Class.AudioTremolo`
- `Class.VideoPlayer`
- `Class.VideoDisplay`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Wire.Connected` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.Wire.SourceInstance` | `Class.Instance` |  |
| `Class.Wire.SourceName` | `string` |  |
| `Class.Wire.TargetInstance` | `Class.Instance` |  |
| `Class.Wire.TargetName` | `string` |  |

## Methods

### `Class.Wire:RenameToDefault`

``RenameToDefault()`` -> `null`
   {security: RobloxScriptSecurity}
