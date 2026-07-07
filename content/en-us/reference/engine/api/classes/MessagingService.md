---
title: MessagingService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# MessagingService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **PublishAsync**(`topic: string`, `message: Variant`) -> `null` [Yields]
- **SubscribeAsync**(`topic: string`, `callback: Function`) -> `RBXScriptConnection` [Yields]
