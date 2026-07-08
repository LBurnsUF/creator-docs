---
title: KeyframeSequenceProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# KeyframeSequenceProvider

Provides functions to load and preview `Class.KeyframeSequence`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The **KeyframeSequenceProvider** service provides functions to load and
preview `Class.KeyframeSequence|KeyframeSequences`. It includes a number of
functions that are useful when working with `Class.Animation|Animations`.

A `Class.KeyframeSequence` stores a series of `Class.Pose|Poses` that encode
the hierarchy and motion of an animation. The animation data Roblox uses in
the playback of an animation, referenced by the `Class.Animation.AnimationId`
property, can be constructed from a `Class.KeyframeSequence`.
`Class.KeyframeSequence|KeyframeSequences` are usually created by the Roblox
[Animation Editor](../../../animation/editor.md) but can be created through
other plugins or even manually.

> **Deprecated:** This service is deprecated and does not support the newer
`Class.AnimationClip`. It's recommended to use `Class.AnimationClipProvider`
instead.

## Methods

### `Class.KeyframeSequenceProvider:GetAnimations`

``GetAnimations(userId: `Datatype.User`)`` -> `Class.Instance`
  [Yields] [Deprecated]

### `Class.KeyframeSequenceProvider:GetAnimationsAsync`

``GetAnimationsAsync(userId: `Datatype.User`)`` -> `Class.Instance`
  [Yields]

### `Class.KeyframeSequenceProvider:GetKeyframeSequence`

``GetKeyframeSequence(assetId: `Datatype.ContentId`)`` -> `Class.Instance`
  [Deprecated] {security: PluginSecurity}

### `Class.KeyframeSequenceProvider:GetKeyframeSequenceAsync`

``GetKeyframeSequenceAsync(assetId: `Datatype.ContentId`)`` -> `Class.Instance`
  [Yields]

### `Class.KeyframeSequenceProvider:GetKeyframeSequenceById`

``GetKeyframeSequenceById(assetId: `int64`, useCache: `bool`)`` -> `Class.Instance`
  [Deprecated] {security: PluginSecurity}

### `Class.KeyframeSequenceProvider:GetMemStats`

``GetMemStats()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.KeyframeSequenceProvider:RegisterActiveKeyframeSequence`

``RegisterActiveKeyframeSequence(keyframeSequence: `Class.Instance`)`` -> `Datatype.ContentId`

### `Class.KeyframeSequenceProvider:RegisterKeyframeSequence`

``RegisterKeyframeSequence(keyframeSequence: `Class.Instance`)`` -> `Datatype.ContentId`
