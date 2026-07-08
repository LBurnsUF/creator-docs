---
title: GamepadService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# GamepadService

The GamepadService is internally responsible for handling inputs from various
controllers, such as Xbox One or PlayStation DualShock controllers.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

The GamepadService is internally responsible for handling inputs from various
controllers, such as Xbox One or PlayStation DualShock controllers. It also
handles APIs used with the gamepad virtual cursor. You can enable the gamepad
cursor for your experience by setting `Enum.VirtualCursorMode` under
`Class.StarterGui|StarterGui` to `Enabled`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.GamepadService.GamepadCursorEnabled` | `bool` |  {write: RobloxScriptSecurity} |

## Methods

### `Class.GamepadService:AutoSelectGui`

``AutoSelectGui()`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.GamepadService:DisableGamepadCursor`

``DisableGamepadCursor()`` -> `null`

### `Class.GamepadService:EnableGamepadCursor`

``EnableGamepadCursor(guiObject: `Class.Instance`)`` -> `null`

### `Class.GamepadService:GetGamepadCursorPosition`

``GetGamepadCursorPosition()`` -> `Datatype.Vector2`
   {security: RobloxScriptSecurity}

### `Class.GamepadService:SetGamepadCursorPosition`

``SetGamepadCursorPosition(position: `Datatype.Vector2`)`` -> `null`
   {security: RobloxScriptSecurity}

## Events

### `Class.GamepadService.GamepadThumbstick1Changed`

Fires with: (event: `Datatype.Vector2`)
