---
title: StudioDeviceSimulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioDeviceSimulatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Methods

- **CreateDeviceAsync**(`config: Dictionary`) -> `string` [Yields]
- **GetDeviceAsync**() -> `string` [Yields]
- **GetDeviceInfoAsync**(`deviceId: string`) -> `Dictionary` [Yields]
- **GetDeviceListAsync**() -> `Array` [Yields]
- **GetOrientationAsync**() -> `ScreenOrientation` [Yields]
- **GetPixelDensityAsync**() -> `float` [Yields]
- **GetResolutionAsync**() -> `Vector2` [Yields]
- **GetScalingModeAsync**() -> `DeviceSimulatorScalingMode` [Yields]
- **RemoveDeviceAsync**(`deviceId: string`) -> `null` [Yields]
- **SetDeviceAsync**(`deviceId: string`) -> `null` [Yields]
- **SetOrientationAsync**(`orientation: ScreenOrientation`) -> `null` [Yields]
- **SetPixelDensityAsync**(`density: float`) -> `null` [Yields]
- **SetResolutionAsync**(`width: int`, `height: int`) -> `null` [Yields]
- **SetScalingModeAsync**(`mode: DeviceSimulatorScalingMode`) -> `null` [Yields]
- **StopSimulationAsync**() -> `null` [Yields]
- **UpdateDeviceAsync**(`deviceId: string`, `config: Dictionary`) -> `null` [Yields]

## Events

- **ConfigurationChanged**()
