---
title: KeyframeSequenceProvider
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# KeyframeSequenceProvider

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetAnimations**(`userId: User`) -> `Instance` [Yields] [Deprecated]
- **GetAnimationsAsync**(`userId: User`) -> `Instance` [Yields]
- **GetKeyframeSequence**(`assetId: ContentId`) -> `Instance` [Deprecated]
- **GetKeyframeSequenceAsync**(`assetId: ContentId`) -> `Instance` [Yields]
- **GetKeyframeSequenceById**(`assetId: int64`, `useCache: bool`) -> `Instance` [Deprecated]
- **GetMemStats**() -> `Dictionary`
- **RegisterActiveKeyframeSequence**(`keyframeSequence: Instance`) -> `ContentId`
- **RegisterKeyframeSequence**(`keyframeSequence: Instance`) -> `ContentId`
