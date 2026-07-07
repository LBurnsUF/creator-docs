---
title: AudioFocusService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AudioFocusService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **AcquireFocus**(`contextId: int`) -> `bool`
- **GetFocusedContextId**() -> `int`
- **GetRegisteredContexts**() -> `Array`
- **RegisterContextIdFromLua**(`contextId: int`) -> `null`
- **RequestFocus**(`contextId: int`, `priority: int`) -> `bool`

## Events

- **OnContextRegistered**(`contextId: int`)
- **OnContextUnregistered**(`contextId: int`)
- **OnDeafenVoiceAudio**(`contextId: int`)
- **OnUndeafenVoiceAudio**(`contextId: int`)
