---
title: StudioDeviceSimulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioDeviceSimulatorService

Service allowing you to control Studio's Device Simulator.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

Provides programmatic control over Studio's Device Simulator. Use this service
to switch between device presets, override resolution and pixel density,
control orientation and scaling, and manage custom device profiles from a
plugin or from an external tool connected through the MCP server.

All methods are asynchronous and yield the calling coroutine. The service is
available in **Edit mode** and **Play Client**. Methods that modify the active
simulation state are blocked in **PlayServer** mode.

##### Limitations

- All methods are asynchronous and yield the calling coroutine.
- Methods that modify the active simulation state (`SetDeviceAsync`,
  `StopSimulationAsync`, `SetOrientationAsync`, `SetResolutionAsync`,
  `SetPixelDensityAsync`, `SetScalingModeAsync`) error in PlayServer mode.
  They work in Edit mode and Play Client.
- `UpdateDeviceAsync` and `RemoveDeviceAsync` error when called on built-in
  presets.
- Resolution, DPI, and scaling mode methods require an active device and error
  when `GetDeviceAsync()` returns "default".
- Resolution and DPI overrides are session-level. They are not persisted and
  are cleared on `SetDeviceAsync`.
- Built-in presets are immutable.

## Methods

### `Class.StudioDeviceSimulatorService:CreateDeviceAsync`

``CreateDeviceAsync(config: `Dictionary`)`` -> `string`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceAsync`

``GetDeviceAsync()`` -> `string`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceInfoAsync`

``GetDeviceInfoAsync(deviceId: `string`)`` -> `Dictionary`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceListAsync`

``GetDeviceListAsync()`` -> `Array`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetOrientationAsync`

``GetOrientationAsync()`` -> `Enum.ScreenOrientation`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetPixelDensityAsync`

``GetPixelDensityAsync()`` -> `float`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetResolutionAsync`

``GetResolutionAsync()`` -> `Datatype.Vector2`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetScalingModeAsync`

``GetScalingModeAsync()`` -> `Enum.DeviceSimulatorScalingMode`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:RemoveDeviceAsync`

``RemoveDeviceAsync(deviceId: `string`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetDeviceAsync`

``SetDeviceAsync(deviceId: `string`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetOrientationAsync`

``SetOrientationAsync(orientation: `Enum.ScreenOrientation`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetPixelDensityAsync`

``SetPixelDensityAsync(density: `float`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetResolutionAsync`

``SetResolutionAsync(width: `int`, height: `int`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetScalingModeAsync`

``SetScalingModeAsync(mode: `Enum.DeviceSimulatorScalingMode`)`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:StopSimulationAsync`

``StopSimulationAsync()`` -> `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:UpdateDeviceAsync`

``UpdateDeviceAsync(deviceId: `string`, config: `Dictionary`)`` -> `null`
  [Yields] {security: PluginSecurity}

## Events

### `Class.StudioDeviceSimulatorService.ConfigurationChanged`

Fires with: ()
