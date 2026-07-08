---
title: NumberRange
type: datatype
---

# `Datatype.NumberRange`

Represents a range of numbers.

## Description

The `Datatype.NumberRange` represents a range of numbers.

`NumberRange` stores its `Datatype.NumberRange.Min` and
`Datatype.NumberRange.Max` values as 32-bit floating-point numbers. Very large
numbers or numbers requiring high decimal precision may lose accuracy.

## Constructors

### `NumberRange.new`

Returns a new `Datatype.NumberRange` with the minimum and maximum set to the
`value`.

**Parameters:**

- `value`: `number`

### `NumberRange.new`

Returns a new `Datatype.NumberRange` with the provided `minimum` and `maximum`. The
`minimum` must be less than or equal to `maximum`.

**Parameters:**

- `minimum`: `number`
- `maximum`: `number`

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `NumberRange.Min` | `number` | The minimum value of the `Datatype.NumberRange`. |
| `NumberRange.Max` | `number` | The maximum value of the `Datatype.NumberRange`. |

## API Usage (25 locations)

### Used as Property Type

- `Class.AudioEqualizer.MidRange`
- `Class.AudioGate.Threshold`
- `Class.AudioPlayer.LoopRegion`
- `Class.AudioPlayer.PlaybackRegion`
- `Class.AvatarBodyRules.CustomBodyTypeScale`
- `Class.AvatarBodyRules.CustomHeadScale`
- `Class.AvatarBodyRules.CustomHeight`
- `Class.AvatarBodyRules.CustomHeightScale`
- `Class.AvatarBodyRules.CustomProportionsScale`
- `Class.AvatarBodyRules.CustomWidthScale`
- `Class.ParticleEmitter.FlipbookFramerate`
- `Class.ParticleEmitter.Lifetime`
- `Class.ParticleEmitter.RotSpeed`
- `Class.ParticleEmitter.Rotation`
- `Class.ParticleEmitter.Speed`
- `Class.Sound.LoopRegion`
- `Class.Sound.PlaybackRegion`
- `Class.StarterPlayer.GameSettingsScaleRangeBodyType`
- `Class.StarterPlayer.GameSettingsScaleRangeHead`
- `Class.StarterPlayer.GameSettingsScaleRangeHeight`
- `Class.StarterPlayer.GameSettingsScaleRangeProportion`
- `Class.StarterPlayer.GameSettingsScaleRangeWidth`
- `Class.StyleQuery.AspectRatioRange`

### Used as Parameter Type

- `Class.AudioPlayer:GetWaveformAsync` (parameter `timeRange`)
- `Class.AudioTextToSpeech:GetWaveformAsync` (parameter `timeRange`)
