---
title: ModerationService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# ModerationService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **BindReviewableContentEventProcessor**(`priority: int`, `callback: Function`) -> `RBXScriptConnection`
- **CreateReviewableContentAsync**(`config: Dictionary`) -> `string` [Yields]
- **CreateReviewableContentKey**(`content: Content`) -> `string`
- **InternalRequestReviewableContentReviewAsync**(`config: Dictionary`) -> `null` [Yields]
