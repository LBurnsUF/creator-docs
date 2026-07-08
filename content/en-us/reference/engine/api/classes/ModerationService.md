---
title: ModerationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ModerationService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.ModerationService:BindReviewableContentEventProcessor`

``BindReviewableContentEventProcessor(priority: `int`, callback: `Datatype.Function`)`` -> `Datatype.RBXScriptConnection`

### `Class.ModerationService:CreateReviewableContentAsync`

``CreateReviewableContentAsync(config: `Dictionary`)`` -> `string`
  [Yields]

### `Class.ModerationService:CreateReviewableContentKey`

``CreateReviewableContentKey(content: `Datatype.Content`)`` -> `string`

### `Class.ModerationService:InternalRequestReviewableContentReviewAsync`

``InternalRequestReviewableContentReviewAsync(config: `Dictionary`)`` -> `null`
  [Yields]
