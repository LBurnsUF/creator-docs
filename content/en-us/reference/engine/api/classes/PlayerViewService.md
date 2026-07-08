---
title: PlayerViewService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# PlayerViewService

Provides a way to get additional information about a player's view.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`Class.PlayerViewService` provides a way to get additional information about a
player's view.

## Methods

### `Class.PlayerViewService:GetDeviceCameraCFrame`

``GetDeviceCameraCFrame(player: `Class.Player`)`` -> `Datatype.CFrame`

### `Class.PlayerViewService:GetDeviceCameraCFrameForSelfView`

``GetDeviceCameraCFrameForSelfView()`` -> `Datatype.CFrame`
   {security: RobloxScriptSecurity}

### `Class.PlayerViewService:OnCameraCFrameReplicationRequest`

``OnCameraCFrameReplicationRequest()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.PlayerViewService:UpdateDeviceCFrame`

``UpdateDeviceCFrame(player: `Class.Player`, cframe: `Datatype.CFrame`, timestamp: `int64`)`` -> `null`
   {security: RobloxScriptSecurity}
