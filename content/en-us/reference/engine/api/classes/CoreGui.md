---
title: CoreGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service, NotReplicated]
---

# CoreGui

**Inherits**: BasePlayerGui > Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **SelectionImageObject**: `GuiObject` (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **Version**: `int` [ReadOnly] [NotReplicated]

## Methods

- **SetUserGuiRendering**(`enabled: bool`, `guiAdornee: Instance`, `faceId: NormalId`, `horizontalCurvature: float = 0`) -> `null`
- **TakeScreenshot**() -> `null`
- **ToggleRecording**() -> `null`

## Events

- **UserGuiRenderingChanged**(`enabled: bool`, `guiAdornee: Instance`, `faceId: NormalId`, `horizontalCurvature: float`)
