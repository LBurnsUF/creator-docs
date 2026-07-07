---
title: FacialAnimationStreamingServiceV2
type: class
superclass: Instance
tags: [NotCreatable, Service]
---

# FacialAnimationStreamingServiceV2

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service

## Properties

- **ServiceState**: `int` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **GetStats**() -> `FacialAnimationStreamingServiceStats`
- **IsAudioEnabled**(`mask: int`) -> `bool`
- **IsPlaceEnabled**(`mask: int`) -> `bool`
- **IsServerEnabled**(`mask: int`) -> `bool`
- **IsVideoEnabled**(`mask: int`) -> `bool`
- **ResolveStateForUser**(`userId: int64`) -> `int` [Yields]
