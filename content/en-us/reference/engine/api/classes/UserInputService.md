---
title: UserInputService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# UserInputService

`UserInputService` is primarily used to detect the input types available on a
user's device, as well as detect input events.

**Inherits from:** `Class.Instance` > `Class.Object`

**Tags:** [NotCreatable] [Service] [NotReplicated]

## Description

`UserInputService` is primarily used to detect the input types available on a
user's device, as well as detect input events. It allows you to perform
different actions depending on the device and, in turn, provide the best
experience for the end user.

As this service is intended for client-side usage only, its properties,
methods, and events can only be used in a `Class.LocalScript`, a
`Class.ModuleScript` required by a `Class.LocalScript`, or a `Class.Script`
with `Class.BaseScript.RunContext|RunContext` set to `Enum.RunContext.Client`.

## Properties

| Property | Type | Description |
|----------|------|-------------|
| `Class.UserInputService.AccelerometerEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.BottomBarSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.GamepadEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.GyroscopeEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.KeyboardEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.LegacyInputEventsEnabled` | `bool` | [Hidden] [Deprecated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.ModalEnabled` | `bool` | [Deprecated] |
| `Class.UserInputService.MouseBehavior` | `Enum.MouseBehavior` |  |
| `Class.UserInputService.MouseDeltaSensitivity` | `float` | [NotReplicated] |
| `Class.UserInputService.MouseEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.MouseIcon` | `Datatype.ContentId` |  |
| `Class.UserInputService.MouseIconContent` | `Datatype.Content` |  |
| `Class.UserInputService.MouseIconEnabled` | `bool` |  |
| `Class.UserInputService.NavBarSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.OnScreenKeyboardAnimationDuration` | `double` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.OnScreenKeyboardPosition` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.OnScreenKeyboardSize` | `Datatype.Vector2` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.OnScreenKeyboardVisible` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.OverrideMouseIconBehavior` | `Enum.OverrideMouseIconBehavior` | [Hidden] {security: RobloxScriptSecurity} |
| `Class.UserInputService.PreferredInput` | `Enum.PreferredInput` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.RightBarSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.StatusBarSize` | `Datatype.Vector2` | [Hidden] [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.TouchEnabled` | `bool` | [ReadOnly] [NotReplicated] |
| `Class.UserInputService.TouchScreenEnabled` | `bool` | [ReadOnly] [NotReplicated] {security: RobloxScriptSecurity} |
| `Class.UserInputService.UserHeadCFrame` | `Datatype.CFrame` | [ReadOnly] [NotReplicated] [Deprecated] |
| `Class.UserInputService.VREnabled` | `bool` | [ReadOnly] [NotReplicated] |

## Methods

### `Class.UserInputService:CreateVirtualInput`

``CreateVirtualInput()`` -> `Class.Object`

### `Class.UserInputService:GamepadSupports`

``GamepadSupports(gamepadNum: `Enum.UserInputType`, gamepadKeyCode: `Enum.KeyCode`)`` -> `bool`

### `Class.UserInputService:GetConnectedGamepads`

``GetConnectedGamepads()`` -> `Array`

### `Class.UserInputService:GetDeviceAcceleration`

``GetDeviceAcceleration()`` -> `Class.InputObject`

### `Class.UserInputService:GetDeviceGravity`

``GetDeviceGravity()`` -> `Class.InputObject`

### `Class.UserInputService:GetDeviceLevel`

``GetDeviceLevel()`` -> `Enum.DeviceLevel`
   {security: RobloxScriptSecurity}

### `Class.UserInputService:GetDeviceRotation`

``GetDeviceRotation()`` -> `Tuple`

### `Class.UserInputService:GetDeviceType`

``GetDeviceType()`` -> `Enum.DeviceType`
   {security: RobloxScriptSecurity}

### `Class.UserInputService:GetFocusedTextBox`

``GetFocusedTextBox()`` -> `Class.TextBox`

### `Class.UserInputService:GetGamepadConnected`

``GetGamepadConnected(gamepadNum: `Enum.UserInputType`)`` -> `bool`

### `Class.UserInputService:GetGamepadState`

``GetGamepadState(gamepadNum: `Enum.UserInputType`)`` -> `Datatype.Instances`

### `Class.UserInputService:GetImageForKeyCode`

``GetImageForKeyCode(keyCode: `Enum.KeyCode`)`` -> `Datatype.ContentId`

### `Class.UserInputService:GetKeysPressed`

``GetKeysPressed()`` -> `Datatype.Instances`

### `Class.UserInputService:GetLastInputType`

``GetLastInputType()`` -> `Enum.UserInputType`

### `Class.UserInputService:GetMouseButtonsPressed`

``GetMouseButtonsPressed()`` -> `Datatype.Instances`

### `Class.UserInputService:GetMouseDelta`

``GetMouseDelta()`` -> `Datatype.Vector2`

### `Class.UserInputService:GetMouseLocation`

``GetMouseLocation()`` -> `Datatype.Vector2`

### `Class.UserInputService:GetNavigationGamepads`

``GetNavigationGamepads()`` -> `Array`

### `Class.UserInputService:GetPasteText`

``GetPasteText()`` -> `string`
   {security: RobloxScriptSecurity}

### `Class.UserInputService:GetPlatform`

``GetPlatform()`` -> `Enum.Platform`
   {security: RobloxScriptSecurity}

### `Class.UserInputService:GetStringForKeyCode`

``GetStringForKeyCode(keyCode: `Enum.KeyCode`, format: `Enum.KeyCodeStringFormat`)`` -> `string`

### `Class.UserInputService:GetSupportedGamepadKeyCodes`

``GetSupportedGamepadKeyCodes(gamepadNum: `Enum.UserInputType`)`` -> `Array`

### `Class.UserInputService:GetUserCFrame`

``GetUserCFrame(type: `Enum.UserCFrame`)`` -> `Datatype.CFrame`
  [Deprecated]

### `Class.UserInputService:IsGamepadButtonDown`

``IsGamepadButtonDown(gamepadNum: `Enum.UserInputType`, gamepadKeyCode: `Enum.KeyCode`)`` -> `bool`

### `Class.UserInputService:IsKeyDown`

``IsKeyDown(keyCode: `Enum.KeyCode`)`` -> `bool`

### `Class.UserInputService:IsMouseButtonPressed`

``IsMouseButtonPressed(mouseButton: `Enum.UserInputType`)`` -> `bool`

### `Class.UserInputService:IsNavigationGamepad`

``IsNavigationGamepad(gamepadEnum: `Enum.UserInputType`)`` -> `bool`

### `Class.UserInputService:RecenterUserHeadCFrame`

``RecenterUserHeadCFrame()`` -> `null`

### `Class.UserInputService:SendAppUISizes`

``SendAppUISizes(statusBarSize: `Datatype.Vector2`, navBarSize: `Datatype.Vector2`, bottomBarSize: `Datatype.Vector2`, rightBarSize: `Datatype.Vector2`)`` -> `null`
   {security: RobloxScriptSecurity}

### `Class.UserInputService:SetNavigationGamepad`

``SetNavigationGamepad(gamepadEnum: `Enum.UserInputType`, enabled: `bool`)`` -> `null`

## Events

### `Class.UserInputService.DeviceAccelerationChanged`

Fires with: (acceleration: `Class.InputObject`)

### `Class.UserInputService.DeviceGravityChanged`

Fires with: (gravity: `Class.InputObject`)

### `Class.UserInputService.DeviceRotationChanged`

Fires with: (rotation: `Class.InputObject`, cframe: `Datatype.CFrame`)

### `Class.UserInputService.GamepadConnected`

Fires with: (gamepadNum: `Enum.UserInputType`)

### `Class.UserInputService.GamepadDisconnected`

Fires with: (gamepadNum: `Enum.UserInputType`)

### `Class.UserInputService.InputBegan`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.InputChanged`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.InputEnded`

Fires with: (input: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.JumpRequest`

Fires with: ()

### `Class.UserInputService.LastInputTypeChanged`

Fires with: (lastInputType: `Enum.UserInputType`)

### `Class.UserInputService.PointerAction`

Fires with: (wheel: `float`, pan: `Datatype.Vector2`, pinch: `float`, gameProcessedEvent: `bool`)

### `Class.UserInputService.StatusBarTapped`

Fires with: (position: `Datatype.Vector2`)

### `Class.UserInputService.TextBoxFocusReleased`

Fires with: (textboxReleased: `Class.TextBox`)

### `Class.UserInputService.TextBoxFocused`

Fires with: (textboxFocused: `Class.TextBox`)

### `Class.UserInputService.TouchDrag`

Fires with: (dragDirection: `Enum.SwipeDirection`, numberOfTouches: `int`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchEnded`

Fires with: (touch: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchLongPress`

Fires with: (touchPositions: `Array`, state: `Enum.UserInputState`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchMoved`

Fires with: (touch: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchPan`

Fires with: (touchPositions: `Array`, totalTranslation: `Datatype.Vector2`, velocity: `Datatype.Vector2`, state: `Enum.UserInputState`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchPinch`

Fires with: (touchPositions: `Array`, scale: `float`, velocity: `float`, state: `Enum.UserInputState`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchRotate`

Fires with: (touchPositions: `Array`, rotation: `float`, velocity: `float`, state: `Enum.UserInputState`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchStarted`

Fires with: (touch: `Class.InputObject`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchSwipe`

Fires with: (swipeDirection: `Enum.SwipeDirection`, numberOfTouches: `int`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchTap`

Fires with: (touchPositions: `Array`, gameProcessedEvent: `bool`)

### `Class.UserInputService.TouchTapInWorld`

Fires with: (position: `Datatype.Vector2`, processedByUI: `bool`)

### `Class.UserInputService.UserCFrameChanged`

Fires with: (type: `Enum.UserCFrame`, value: `Datatype.CFrame`)
  [Deprecated]

### `Class.UserInputService.WindowFocusReleased`

Fires with: ()

### `Class.UserInputService.WindowFocused`

Fires with: ()
