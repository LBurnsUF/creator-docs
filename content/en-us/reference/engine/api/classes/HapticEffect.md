---
title: HapticEffect
type: class
superclass: Instance
---

# HapticEffect

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

Modern controllers and devices have motors built‑in to provide haptic
feedback. Adding rumbles and vibrations can provide subtle feedback that is
hard to convey through visuals or audio.

Roblox supports haptics for the following devices:

- Android and iOS phones supporting haptics including most iPhone, Pixel, and
  Samsung Galaxy devices
- PlayStation gamepads
- Xbox gamepads
- Quest Touch controller

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.HapticEffect.Looped` | `bool` |  |
| `Class.HapticEffect.Position` | `Datatype.Vector3` |  |
| `Class.HapticEffect.Radius` | `float` |  |
| `Class.HapticEffect.Type` | `Enum.HapticEffectType` |  |

## Methods

### `Class.HapticEffect:Play`

``Play()`` -> `null`

### `Class.HapticEffect:SetWaveformKeys`

``SetWaveformKeys(keys: `Array`)`` -> `null`

### `Class.HapticEffect:Stop`

``Stop()`` -> `null`

## Events

### `Class.HapticEffect.Ended`

Fires with: ()
