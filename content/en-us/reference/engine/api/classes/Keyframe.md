---
title: Keyframe
type: class
superclass: Instance
---

# Keyframe

A Keyframe holds the `Class.Pose|Poses` applied to joints in a `Class.Model`
at a given point of time in an animation. `Class.Keyframe|Keyframes` are
interpolated between during animation playback.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A Keyframe holds the `Class.Pose|Poses` applied to joints in a `Class.Model`
at a given point of time in an animation. `Class.Keyframe|Keyframes` are
interpolated between during animation playback.

Note, in most cases developers do not need to manipulate
`Class.KeyframeSequence|KeyframeSequences` as the animation editor covers most
animation functionality. However, in some cases a developer may wish to
generate an animation from a `Class.Script` or build their own plugin.

## Structure

Keyframes are held within a `Class.KeyframeSequence` and contain `Class.Pose`
objects. The poses are named in accordance with the `Class.BasePart|BaseParts`
they correspond to and are structured in terms of joint hierarchy. This means
each `Class.Pose` is parented to the `Class.Pose` corresponding to the part it
is attached to.

Note, as `Class.Pose|Poses` are named in accordance with the
`Class.BasePart|BaseParts` they correspond to, animations require distinct
part names to play correctly.

## Interpolation

During animation playback the poses in different keyframes are interpolated
between. This allows a smooth animation to be created without needing to
define every frame. Note, the style of interpolation is determined in the
`Class.Pose` object. The Keyframe object merely holds the `Class.Pose|Poses`
at a defined point of time in the animation (`Class.Keyframe.Time`).

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.Keyframe.Time` | `float` |  |

## Methods

### `Class.Keyframe:AddMarker`

``AddMarker(marker: `Class.Instance`)`` -> `null`

### `Class.Keyframe:AddPose`

``AddPose(pose: `Class.Instance`)`` -> `null`

### `Class.Keyframe:GetMarkers`

``GetMarkers()`` -> `Datatype.Instances`

### `Class.Keyframe:GetPoses`

``GetPoses()`` -> `Datatype.Instances`

### `Class.Keyframe:RemoveMarker`

``RemoveMarker(marker: `Class.Instance`)`` -> `null`

### `Class.Keyframe:RemovePose`

``RemovePose(pose: `Class.Instance`)`` -> `null`
