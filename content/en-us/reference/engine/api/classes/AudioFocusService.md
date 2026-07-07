---
title: AudioFocusService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# AudioFocusService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.AudioFocusService:AcquireFocus`

``AcquireFocus(contextId: `int`)`` → `bool`
   {security: RobloxScriptSecurity}

### `Class.AudioFocusService:GetFocusedContextId`

``GetFocusedContextId()`` → `int`
   {security: RobloxScriptSecurity}

### `Class.AudioFocusService:GetRegisteredContexts`

``GetRegisteredContexts()`` → `Array`
   {security: RobloxScriptSecurity}

### `Class.AudioFocusService:RegisterContextIdFromLua`

``RegisterContextIdFromLua(contextId: `int`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.AudioFocusService:RequestFocus`

``RequestFocus(contextId: `int`, priority: `int`)`` → `bool`
   {security: RobloxScriptSecurity}

## Events

### `Class.AudioFocusService.OnContextRegistered`

Fires with: (contextId: `int`)

### `Class.AudioFocusService.OnContextUnregistered`

Fires with: (contextId: `int`)

### `Class.AudioFocusService.OnDeafenVoiceAudio`

Fires with: (contextId: `int`)

### `Class.AudioFocusService.OnUndeafenVoiceAudio`

Fires with: (contextId: `int`)
