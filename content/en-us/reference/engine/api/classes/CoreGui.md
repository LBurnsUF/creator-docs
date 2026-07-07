---
title: CoreGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service, NotReplicated]
---

# CoreGui

**Inherits from:** `Class.BasePlayerGui` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Properties

| Property | Type | Tags |
|----------|------|------|
| `Class.CoreGui.SelectionImageObject` | `Class.GuiObject` |  {security: RobloxScriptSecurity} |
| `Class.CoreGui.Version` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.CoreGui:SetUserGuiRendering`

``SetUserGuiRendering(enabled: `bool`, guiAdornee: `Class.Instance`, faceId: `Enum.NormalId`, horizontalCurvature: `float`)`` → `null`
   {security: RobloxScriptSecurity}

### `Class.CoreGui:TakeScreenshot`

``TakeScreenshot()`` → `null`
   {security: RobloxScriptSecurity}

### `Class.CoreGui:ToggleRecording`

``ToggleRecording()`` → `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.CoreGui.UserGuiRenderingChanged`

Fires with: (enabled: `bool`, guiAdornee: `Class.Instance`, faceId: `Enum.NormalId`, horizontalCurvature: `float`)
