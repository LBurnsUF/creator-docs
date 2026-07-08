---
title: CoreGui
type: class
superclass: BasePlayerGui
tags: [NotCreatable, Service, NotReplicated]
---

# CoreGui

The CoreGui is a service used to store Guis created in-game by Roblox for the
core user interface found in every game (such as the game menu, the
playerlist, the backpack, etc.). It can also be used by `Class.Plugin|Plugins`
in Roblox Studio.

**Inherits from:** `Class.BasePlayerGui` > `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The CoreGui is a service used to store Guis created in-game by Roblox for the
core user interface found in every game (such as the game menu, the
playerlist, the backpack, etc.). It can also be used by `Class.Plugin|Plugins`
in Roblox Studio.

You can use the `Class.StarterGui:SetCoreGuiEnabled()` and
`Class.StarterGui:GetCoreGuiEnabled()` methods in a `Class.LocalScript` to
enable and disable most elements of the CoreGui. You can also use
`Class.PlayerGui:SetTopbarTransparency()` to set the transparency of the top
bar.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.CoreGui.SelectionImageObject` | `Class.GuiObject` |  {security: RobloxScriptSecurity} |
| `Class.CoreGui.Version` | `int` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.CoreGui:SetUserGuiRendering`

``SetUserGuiRendering(enabled: `bool`, guiAdornee: `Class.Instance`, faceId: `Enum.NormalId`, horizontalCurvature: `float`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CoreGui:TakeScreenshot`

``TakeScreenshot()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.CoreGui:ToggleRecording`

``ToggleRecording()`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.CoreGui.UserGuiRenderingChanged`

Fires with: (enabled: `bool`, guiAdornee: `Class.Instance`, faceId: `Enum.NormalId`, horizontalCurvature: `float`)
