---
title: StudioCameraService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# StudioCameraService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **FocusDistance**: `float` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LockCameraSpeed**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **LoggingEnabled**: `bool` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)

## Methods

- **InFocusMode**() -> `bool`
- **InterpolateView**(`target: CFrame`) -> `null`
- **SetFocusLock**(`value: bool`) -> `null`

## Events

- **FocusStateChanged**()
- **OnMouseCaptureBegin**()
- **OnMouseCaptureEnd**()
- **PointFocused**(`point: Vector3`)
- **ShowCameraSpeed**(`speed: float`)
- **UpdateUI**(`deltaTime: double`)
