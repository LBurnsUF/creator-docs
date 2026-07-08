---
title: KeyframeSequence
type: class
superclass: AnimationClip
---

# KeyframeSequence

This object stores all of the `Class.Keyframe|Keyframes` and other data for
the animation.

**Inherits from:** `Class.AnimationClip` > `Class.Instance` > `Class.Object`

## Description

`Class.KeyframeSequence` stores all the `Class.Keyframe|Keyframes` for an
`Class.Animation`, determines if the animation will
`Class.KeyframeSequence.Loop|Loop`, and determines its
`Class.KeyframeSequence.Priority|Priority` against other animations. The last
`Class.Keyframe` in the sequence, meaning the `Class.Keyframe` with the
highest `Class.Keyframe.Time|Time` property, determines the length of an
animation.

Although `Class.KeyframeSequence.Priority|Priority` and
`Class.KeyframeSequence.Loop|Loop` save the priority and looped animation
settings for the sequence, note that `Class.AnimationTrack` properties can
eventually overwrite these properties at playback time.

If you want to preview an `Class.Animation` before uploading it to Roblox, you
can generate a temporary hash ID using
`Class.KeyframeSequenceProvider:RegisterKeyframeSequence()` for localized
animation testing.

#### Obtaining Sequences

In some cases you may wish to download the `Class.KeyframeSequence`
corresponding to an existing uploaded `Class.Animation`. You can use
`Class.AnimationClipProvider:GetAnimationClipAsync()` to download an
animation.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.KeyframeSequence.AuthoredHipHeight` | `float` | [Hidden] {security: PluginSecurity} |

## Methods

### `Class.KeyframeSequence:AddKeyframe`

``AddKeyframe(keyframe: `Class.Instance`)`` -> `null`

### `Class.KeyframeSequence:GetKeyframes`

``GetKeyframes()`` -> `Datatype.Instances`

### `Class.KeyframeSequence:RemoveKeyframe`

``RemoveKeyframe(keyframe: `Class.Instance`)`` -> `null`
