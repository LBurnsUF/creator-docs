---
title: StudioDeviceSimulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioDeviceSimulatorService

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Methods

### `Class.StudioDeviceSimulatorService:CreateDeviceAsync`

``CreateDeviceAsync(config: `Dictionary`)`` → `string`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceAsync`

``GetDeviceAsync()`` → `string`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceInfoAsync`

``GetDeviceInfoAsync(deviceId: `string`)`` → `Dictionary`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetDeviceListAsync`

``GetDeviceListAsync()`` → `Array`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetOrientationAsync`

``GetOrientationAsync()`` → `Enum.ScreenOrientation`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetPixelDensityAsync`

``GetPixelDensityAsync()`` → `float`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetResolutionAsync`

``GetResolutionAsync()`` → `Datatype.Vector2`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:GetScalingModeAsync`

``GetScalingModeAsync()`` → `Enum.DeviceSimulatorScalingMode`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:RemoveDeviceAsync`

``RemoveDeviceAsync(deviceId: `string`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetDeviceAsync`

``SetDeviceAsync(deviceId: `string`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetOrientationAsync`

``SetOrientationAsync(orientation: `Enum.ScreenOrientation`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetPixelDensityAsync`

``SetPixelDensityAsync(density: `float`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetResolutionAsync`

``SetResolutionAsync(width: `int`, height: `int`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:SetScalingModeAsync`

``SetScalingModeAsync(mode: `Enum.DeviceSimulatorScalingMode`)`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:StopSimulationAsync`

``StopSimulationAsync()`` → `null`
  [Yields] {security: PluginSecurity}

### `Class.StudioDeviceSimulatorService:UpdateDeviceAsync`

``UpdateDeviceAsync(deviceId: `string`, config: `Dictionary`)`` → `null`
  [Yields] {security: PluginSecurity}

## Events

### `Class.StudioDeviceSimulatorService.ConfigurationChanged`

Fires with: ()
