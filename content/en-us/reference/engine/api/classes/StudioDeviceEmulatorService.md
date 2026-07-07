---
title: StudioDeviceEmulatorService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioDeviceEmulatorService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **HasMultiTouchStarted**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsMultiTouchEmulationOn**: `bool` [Hidden] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **IsMultiTouchEnabled**: `bool` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PivotPosition**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **EmulatePCDeviceWithResolution**(`deviceId: string`, `resolution: Vector2`) -> `bool` [Yields]
- **GetCurrentDeviceId**() -> `string` [Yields]
- **GetCurrentOrientation**() -> `ScreenOrientation` [Yields]
- **GetMaxNumTouches**() -> `int`
- **GetTouchInBounds**(`index: int`) -> `bool`
- **GetTouchPosition**(`index: int`) -> `Vector2`
- **HasDeviceWithId**(`deviceId: string`) -> `bool` [Yields]
- **SetCurrentDeviceId**(`deviceId: string`) -> `null` [Yields]
- **SetCurrentOrientation**(`orientation: ScreenOrientation`) -> `null` [Yields]

## Events

- **CurrentDeviceIdChanged**()
- **OrientationChanged**()
- **TouchInBoundsChanged**()
- **TouchPositionsChanged**()
