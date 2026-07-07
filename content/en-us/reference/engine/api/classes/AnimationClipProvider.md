---
title: AnimationClipProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AnimationClipProvider

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetAnimationClip**(`assetId: ContentId`) -> `AnimationClip` [Deprecated]
- **GetAnimationClipAsync**(`assetId: ContentId`) -> `AnimationClip` [Yields]
- **GetAnimationClipById**(`assetId: int64`, `useCache: bool`) -> `AnimationClip` [Deprecated]
- **GetAnimationNodeDefinition**(`type: AnimationNodeType`) -> `Dictionary`
- **GetAnimationNodeTypes**() -> `Array`
- **GetAnimations**(`userId: User`) -> `Instance` [Yields] [Deprecated]
- **GetAnimationsAsync**(`userId: User`) -> `Instance` [Yields]
- **GetClipEvaluatorAsync**(`assetId: ContentId`) -> `ClipEvaluator` [Yields]
- **GetMemStats**() -> `Dictionary`
- **RegisterActiveAnimationClip**(`animationClip: AnimationClip`) -> `ContentId`
- **RegisterAnimationClip**(`animationClip: AnimationClip`) -> `ContentId`
