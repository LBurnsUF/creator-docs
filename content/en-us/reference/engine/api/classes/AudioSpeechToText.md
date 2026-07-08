---
title: AudioSpeechToText
type: class
superclass: Instance
---

# AudioSpeechToText

Converts spoken audio into text.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

`Class.AudioSpeechToText` is used to convert speech audio into text. This
class provides a single **Input** pin that can be connected to other pins via
`Class.Wire|Wires`.

Roblox uses the following formula to throttle requests for this API based on
the number of players in your experience:
`max requests per minute per experience = 1 + (5 * number_of_concurrent_users)`.
You can purchase additional usage using
[Extended Services](../../../cloud-services/extended-services.md).

For more information, see
[Speech-to-text](../../../audio/objects.md#speech-to-text).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AudioSpeechToText.DictationEnabled` | `bool` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.AudioSpeechToText.Enabled` | `bool` |  |
| `Class.AudioSpeechToText.Text` | `string` |  |
| `Class.AudioSpeechToText.VoiceDetected` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.AudioSpeechToText:GetConnectedWires`

``GetConnectedWires(pin: `string`)`` -> `Datatype.Instances`

## Events

### `Class.AudioSpeechToText.WiringChanged`

Fires with: (connected: `bool`, pin: `string`, wire: `Class.Wire`, instance: `Class.Instance`)
