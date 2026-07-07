---
title: AnimationClipProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AnimationClipProvider

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AnimationClipProvider:GetAnimationClip`

``GetAnimationClip(assetId: `Datatype.ContentId`)`` → `Class.AnimationClip`
  [Deprecated] {security: PluginSecurity}

### `Class.AnimationClipProvider:GetAnimationClipAsync`

``GetAnimationClipAsync(assetId: `Datatype.ContentId`)`` → `Class.AnimationClip`
  [Yields]

### `Class.AnimationClipProvider:GetAnimationClipById`

``GetAnimationClipById(assetId: `int64`, useCache: `bool`)`` → `Class.AnimationClip`
  [Deprecated] {security: PluginSecurity}

### `Class.AnimationClipProvider:GetAnimationNodeDefinition`

``GetAnimationNodeDefinition(type: `Enum.AnimationNodeType`)`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:GetAnimationNodeTypes`

``GetAnimationNodeTypes()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:GetAnimations`

``GetAnimations(userId: `Datatype.User`)`` → `Class.Instance`
  [Yields] [Deprecated]

### `Class.AnimationClipProvider:GetAnimationsAsync`

``GetAnimationsAsync(userId: `Datatype.User`)`` → `Class.Instance`
  [Yields]

### `Class.AnimationClipProvider:GetClipEvaluatorAsync`

``GetClipEvaluatorAsync(assetId: `Datatype.ContentId`)`` → `Datatype.ClipEvaluator`
  [Yields]

### `Class.AnimationClipProvider:GetMemStats`

``GetMemStats()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.AnimationClipProvider:RegisterActiveAnimationClip`

``RegisterActiveAnimationClip(animationClip: `Class.AnimationClip`)`` → `Datatype.ContentId`

### `Class.AnimationClipProvider:RegisterAnimationClip`

``RegisterAnimationClip(animationClip: `Class.AnimationClip`)`` → `Datatype.ContentId`
