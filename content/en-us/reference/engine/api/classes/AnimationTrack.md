---
title: AnimationTrack
type: class
superclass: Instance
tags: [NotCreatable]
---

# AnimationTrack

Controls the playback of an animation on an `Class.Animator`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable]

## Description

Controls the playback of an animation on an `Class.Animator`. This object
cannot be created, instead it is returned by the
`Class.Animator:LoadAnimation()` method.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AnimationTrack.Animation` | `Class.Animation` | [ReadOnly] [NotReplicated] |
| `Class.AnimationTrack.IsPlaying` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.AnimationTrack.Length` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AnimationTrack.Looped` | `bool` |  |
| `Class.AnimationTrack.Priority` | `Enum.AnimationPriority` |  |
| `Class.AnimationTrack.Speed` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AnimationTrack.TimePosition` | `float` | [NotReplicated] |
| `Class.AnimationTrack.WeightCurrent` | `float` | [ReadOnly] [NotReplicated] |
| `Class.AnimationTrack.WeightTarget` | `float` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.AnimationTrack:AdjustSpeed`

``AdjustSpeed(speed: `float`)`` -> `null`
  [CustomLuaState]

### `Class.AnimationTrack:AdjustWeight`

``AdjustWeight(weight: `float`, fadeTime: `float`)`` -> `null`
  [CustomLuaState]

### `Class.AnimationTrack:GetDebugData`

``GetDebugData()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AnimationTrack:GetMarkerReachedSignal`

``GetMarkerReachedSignal(name: `string`)`` -> `Datatype.RBXScriptSignal`

### `Class.AnimationTrack:GetParameter`

``GetParameter(key: `string`)`` -> `Variant`

### `Class.AnimationTrack:GetParameterDefaults`

``GetParameterDefaults()`` -> `Dictionary`

### `Class.AnimationTrack:GetTargetInstance`

``GetTargetInstance(name: `string`)`` -> `Class.Instance`

### `Class.AnimationTrack:GetTargetNames`

``GetTargetNames()`` -> `Array`

### `Class.AnimationTrack:GetTimeOfKeyframe`

``GetTimeOfKeyframe(keyframeName: `string`)`` -> `double`

### `Class.AnimationTrack:Play`

``Play(fadeTime: `float`, weight: `float`, speed: `float`)`` -> `null`
  [CustomLuaState]

### `Class.AnimationTrack:ResetGraph`

``ResetGraph()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AnimationTrack:SetParameter`

``SetParameter(key: `string`, value: `Variant`)`` -> `null`

### `Class.AnimationTrack:SetTargetInstance`

``SetTargetInstance(name: `string`, target: `Class.Instance`)`` -> `null`

### `Class.AnimationTrack:Stop`

``Stop(fadeTime: `float`)`` -> `null`
  [CustomLuaState]

### `Class.AnimationTrack:UpdateGraphNodeProperty`

``UpdateGraphNodeProperty(nodeId: `string`, propertyName: `string`, value: `Variant`, inputPinName: `string`)`` -> `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.AnimationTrack.DidLoop`

Fires with: ()

### `Class.AnimationTrack.Ended`

Fires with: ()

### `Class.AnimationTrack.KeyframeReached`

Fires with: (keyframeName: `string`)

### `Class.AnimationTrack.Stopped`

Fires with: ()
