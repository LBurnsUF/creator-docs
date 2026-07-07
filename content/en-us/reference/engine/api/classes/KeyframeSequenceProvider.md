---
title: KeyframeSequenceProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# KeyframeSequenceProvider

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.KeyframeSequenceProvider:GetAnimations`

``GetAnimations(userId: `Datatype.User`)`` → `Class.Instance`
  [Yields] [Deprecated]

### `Class.KeyframeSequenceProvider:GetAnimationsAsync`

``GetAnimationsAsync(userId: `Datatype.User`)`` → `Class.Instance`
  [Yields]

### `Class.KeyframeSequenceProvider:GetKeyframeSequence`

``GetKeyframeSequence(assetId: `Datatype.ContentId`)`` → `Class.Instance`
  [Deprecated] {security: PluginSecurity}

### `Class.KeyframeSequenceProvider:GetKeyframeSequenceAsync`

``GetKeyframeSequenceAsync(assetId: `Datatype.ContentId`)`` → `Class.Instance`
  [Yields]

### `Class.KeyframeSequenceProvider:GetKeyframeSequenceById`

``GetKeyframeSequenceById(assetId: `int64`, useCache: `bool`)`` → `Class.Instance`
  [Deprecated] {security: PluginSecurity}

### `Class.KeyframeSequenceProvider:GetMemStats`

``GetMemStats()`` → `Dictionary`
   {security: RobloxScriptSecurity}

### `Class.KeyframeSequenceProvider:RegisterActiveKeyframeSequence`

``RegisterActiveKeyframeSequence(keyframeSequence: `Class.Instance`)`` → `Datatype.ContentId`

### `Class.KeyframeSequenceProvider:RegisterKeyframeSequence`

``RegisterKeyframeSequence(keyframeSequence: `Class.Instance`)`` → `Datatype.ContentId`
