---
title: KeyframeMarker
type: class
superclass: Instance
---

# KeyframeMarker

An instance meant to represent an event that will eventually be fired when a
`Class.Keyframe` is hit.

**Inherits from:** `Class.Instance` > `Class.Object`

## Description

A KeyframeMarker is an instance meant to represent an event that will
eventually be fired when a `Class.Keyframe` is hit.

## Using a KeyframeMarker

KeyframeMarkers should always be parented to a Keyframe via setting the parent
directly or using the `Class.Keyframe:AddMarker()` function of Keyframe.
KeyframeMarkers can also be removed directly or using the
`Class.Keyframe:RemoveMarker()` function, and polled to check which markers
are attached to a specific Keyframe using `Class.Keyframe:GetMarkers()`.

Whenever a Keyframe is detected as an animation is running, there will be an
event fired for each KeyframeMarker that is parented to the Keyframe. These
events are identifiable by the name of the KeyframeMarker. You can retrieve
and listen to these events using the
`Class.AnimationTrack.GetKeyframeMarkerReached` function. Optionally, you may
set the `Class.KeyframeMarker.Value` property of the KeyframeMarker in order
to pass along a value with the event being fired.

It inherits the `Class.Instance.Name|Keyframe.Name` property from
`Class.Instance` and behaves identically. Names are used for identification
and do not need to be unique. When multiple `KeyframeMarker` instances with
the same name are attached to a `Class.Keyframe`, events such as the one
returned by `Class.AnimationTrack:GetMarkerReachedSignal()` will fire for
every marker.

See also:

- `Class.Keyframe`, holds the `Class.Pose|Poses` applied to joints in a
  `Class.Model` at a given point of time in an animation
- `Class.AnimationTrack`, controls the playback of an animation on a
  `Class.Humanoid` or `Class.AnimationController`
- `Class.Animation`, holds a reference to animation data required to play
  custom animations on characters or other models using the Roblox animation
  system

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.KeyframeMarker.Value` | `string` |  |
