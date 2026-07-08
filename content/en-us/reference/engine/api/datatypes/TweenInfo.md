---
title: TweenInfo
type: datatype
---

# `Datatype.TweenInfo`

Stores parameters for `Class.Tween|Tweens`.

## Description

The `Datatype.TweenInfo` data type stores parameters for
`Class.TweenService:Create()` to specify the behavior of the tween. The
properties of a `Datatype.TweenInfo` cannot be written to after its creation.

## Constructors

### `TweenInfo.new`

Creates a new `Datatype.TweenInfo` from the provided parameters.

**Parameters:**

- `time`: `number` - Duration for the tween, in seconds.
- `easingStyle`: `EasingStyle` - Easing style for the tween.
- `easingDirection`: `EasingDirection` - The direction in which the tween executes.
- `repeatCount`: `number` - Number of times the tween should repeat. `-1` repeats indefinitely.
- `reverses`: `bool` - Whether the tween should reverse to the starting values once it
reaches its targets.
- `delayTime`: `number` - Time of delay until the tween begins, in seconds.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `TweenInfo.EasingDirection` | `EasingDirection` | The direction in which the tween executes. |
| `TweenInfo.Time` | `number` | Duration of the tween, in seconds. |
| `TweenInfo.DelayTime` | `number` | Time of delay until the tween begins, in seconds. |
| `TweenInfo.RepeatCount` | `number` | Number of times the tween repeats. |
| `TweenInfo.EasingStyle` | `EasingStyle` | The style in which the tween executes. |
| `TweenInfo.Reverses` | `bool` | Whether or not the tween interpolates in reverse tween once the initial tween completes. |

## API Usage (2 locations)

### Used as Property Type

- `Class.Tween.TweenInfo`

### Used as Parameter Type

- `Class.TweenService:Create` (parameter `tweenInfo`)
