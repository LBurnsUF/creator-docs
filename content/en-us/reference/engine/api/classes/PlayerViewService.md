---
title: PlayerViewService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PlayerViewService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **GetDeviceCameraCFrame**(`player: Player = nil`) -> `CFrame`
- **GetDeviceCameraCFrameForSelfView**() -> `CFrame`
- **OnCameraCFrameReplicationRequest**() -> `null`
- **UpdateDeviceCFrame**(`player: Player = nil`, `cframe: CFrame = 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1`, `timestamp: int64 = 0`) -> `null`
