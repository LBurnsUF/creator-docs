---
title: StudioDeviceEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioDeviceEmulatorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.StudioDeviceEmulatorService.HasMultiTouchStarted` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioDeviceEmulatorService.IsMultiTouchEmulationOn` | `bool` | [Hidden] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioDeviceEmulatorService.IsMultiTouchEnabled` | `bool` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.StudioDeviceEmulatorService.PivotPosition` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |

## Methods

### `Class.StudioDeviceEmulatorService:EmulatePCDeviceWithResolution`

``EmulatePCDeviceWithResolution(deviceId: `string`, resolution: `Datatype.Vector2`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:GetCurrentDeviceId`

``GetCurrentDeviceId()`` -> `string`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:GetCurrentOrientation`

``GetCurrentOrientation()`` -> `Enum.ScreenOrientation`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:GetMaxNumTouches`

``GetMaxNumTouches()`` -> `int`
   {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:GetTouchInBounds`

``GetTouchInBounds(index: `int`)`` -> `bool`
   {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:GetTouchPosition`

``GetTouchPosition(index: `int`)`` -> `Datatype.Vector2`
   {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:HasDeviceWithId`

``HasDeviceWithId(deviceId: `string`)`` -> `bool`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:SetCurrentDeviceId`

``SetCurrentDeviceId(deviceId: `string`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

### `Class.StudioDeviceEmulatorService:SetCurrentOrientation`

``SetCurrentOrientation(orientation: `Enum.ScreenOrientation`)`` -> `null`
  [Yields] {security: RobloxScriptSecurity}

## Events

### `Class.StudioDeviceEmulatorService.CurrentDeviceIdChanged`

Fires with: ()

### `Class.StudioDeviceEmulatorService.OrientationChanged`

Fires with: ()

### `Class.StudioDeviceEmulatorService.TouchInBoundsChanged`

Fires with: ()

### `Class.StudioDeviceEmulatorService.TouchPositionsChanged`

Fires with: ()
