---
title: AnimationStreamTrack
type: class
superclass: Instance
tags: [NotCreatable, NotReplicated]
---

# AnimationStreamTrack

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.AnimationStreamTrack.Animation` | `Class.TrackerStreamAnimation` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.AnimationStreamTrack.FACSDataLod` | `Enum.FACSDataLod` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.AnimationStreamTrack.IsPlaying` | `bool` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.AnimationStreamTrack.Priority` | `Enum.AnimationPriority` | [Hidden] [NotReplicated] |
| `Class.AnimationStreamTrack.WeightCurrent` | `float` | [Hidden] [ReadOnly] [NotReplicated] |
| `Class.AnimationStreamTrack.WeightTarget` | `float` | [Hidden] [ReadOnly] [NotReplicated] |

## Methods

### `Class.AnimationStreamTrack:AdjustWeight`

``AdjustWeight(weight: `float`, fadeTime: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AnimationStreamTrack:GetActive`

``GetActive()`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.AnimationStreamTrack:GetTrackerData`

``GetTrackerData()`` -> `Tuple`
   {security: RobloxScriptSecurity}

### `Class.AnimationStreamTrack:Play`

``Play(fadeTime: `float`, weight: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AnimationStreamTrack:Stop`

``Stop(fadeTime: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.AnimationStreamTrack:TogglePause`

``TogglePause(paused: `bool`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.AnimationStreamTrack.Stopped`

Fires with: ()
