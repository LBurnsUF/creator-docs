---
title: AnimationClipProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AnimationClipProvider

Provides functions to load and preview `Class.AnimationClip|AnimationClips`.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

Provides functions to load and preview `Class.AnimationClip|AnimationClips`.
It includes a number of functions that are useful when working with an
`Class.Animation`.

The `Class.AnimationClipProvider` replaces the deprecated
`Class.KeyframeSequenceProvider` that was used to download `KeyframeSequences`
by content ID.

The AnimationClipProvider has a number of uses.

- Download the `Class.AnimationClip` associated with an animation content ID
  from the Roblox website, regardless of the underlying type of
  `Class.AnimationClip` (`Class.KeyframeSequence` or `Class.CurveAnimation`).
- Generate a temporary ID to locally preview an animation.
- Fetch the content IDs of animations owned by a particular user.

## Methods

### `Class.AnimationClipProvider:GetAnimationClip`

``GetAnimationClip(assetId: `Datatype.ContentId`)`` -> `Class.AnimationClip`
  [Deprecated] {security: PluginSecurity}

### `Class.AnimationClipProvider:GetAnimationClipAsync`

``GetAnimationClipAsync(assetId: `Datatype.ContentId`)`` -> `Class.AnimationClip`
  [Yields]

### `Class.AnimationClipProvider:GetAnimationClipById`

``GetAnimationClipById(assetId: `int64`, useCache: `bool`)`` -> `Class.AnimationClip`
  [Deprecated] {security: PluginSecurity}

### `Class.AnimationClipProvider:GetAnimationNodeDefinition`

``GetAnimationNodeDefinition(type: `Enum.AnimationNodeType`)`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:GetAnimationNodeTypes`

``GetAnimationNodeTypes()`` -> `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:GetAnimations`

``GetAnimations(userId: `Datatype.User`)`` -> `Class.Instance`
  [Yields] [Deprecated]

### `Class.AnimationClipProvider:GetAnimationsAsync`

``GetAnimationsAsync(userId: `Datatype.User`)`` -> `Class.Instance`
  [Yields]

### `Class.AnimationClipProvider:GetClipEvaluatorAsync`

``GetClipEvaluatorAsync(assetId: `Datatype.ContentId`)`` -> `Datatype.ClipEvaluator`
  [Yields]

### `Class.AnimationClipProvider:GetMemStats`

``GetMemStats()`` -> `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:RegisterActiveAnimationClip`

``RegisterActiveAnimationClip(animationClip: `Class.AnimationClip`)`` -> `Datatype.ContentId`

### `Class.AnimationClipProvider:RegisterAnimationClip`

``RegisterAnimationClip(animationClip: `Class.AnimationClip`)`` -> `Datatype.ContentId`
