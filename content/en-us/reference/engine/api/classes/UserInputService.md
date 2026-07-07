---
title: UserInputService
type: class
superclass: Instance
tags: [NotCreatable, Service, NotReplicated]
---

# UserInputService

**Inherits**: Instance > Object

**Tags**: NotCreatable, Service, NotReplicated

## Properties

- **AccelerometerEnabled**: `bool` [ReadOnly] [NotReplicated]
- **BottomBarSize**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **GamepadEnabled**: `bool` [ReadOnly] [NotReplicated]
- **GyroscopeEnabled**: `bool` [ReadOnly] [NotReplicated]
- **KeyboardEnabled**: `bool` [ReadOnly] [NotReplicated]
- **LegacyInputEventsEnabled**: `bool` [Hidden] [Deprecated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **ModalEnabled**: `bool` [Deprecated]
- **MouseBehavior**: `MouseBehavior`
- **MouseDeltaSensitivity**: `float` [NotReplicated]
- **MouseEnabled**: `bool` [ReadOnly] [NotReplicated]
- **MouseIcon**: `ContentId`
- **MouseIconContent**: `Content`
- **MouseIconEnabled**: `bool`
- **NavBarSize**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **OnScreenKeyboardAnimationDuration**: `double` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **OnScreenKeyboardPosition**: `Vector2` [ReadOnly] [NotReplicated]
- **OnScreenKeyboardSize**: `Vector2` [ReadOnly] [NotReplicated]
- **OnScreenKeyboardVisible**: `bool` [ReadOnly] [NotReplicated]
- **OverrideMouseIconBehavior**: `OverrideMouseIconBehavior` [Hidden] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **PreferredInput**: `PreferredInput` [ReadOnly] [NotReplicated]
- **RightBarSize**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **StatusBarSize**: `Vector2` [Hidden] [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **TouchEnabled**: `bool` [ReadOnly] [NotReplicated]
- **TouchScreenEnabled**: `bool` [ReadOnly] [NotReplicated] (Security: Read=RobloxScriptSecurity, Write=RobloxScriptSecurity)
- **UserHeadCFrame**: `CFrame` [ReadOnly] [NotReplicated] [Deprecated]
- **VREnabled**: `bool` [ReadOnly] [NotReplicated]

## Methods

- **CreateVirtualInput**() -> `Object`
- **GamepadSupports**(`gamepadNum: UserInputType`, `gamepadKeyCode: KeyCode`) -> `bool`
- **GetConnectedGamepads**() -> `Array`
- **GetDeviceAcceleration**() -> `InputObject`
- **GetDeviceGravity**() -> `InputObject`
- **GetDeviceLevel**() -> `DeviceLevel`
- **GetDeviceRotation**() -> `Tuple`
- **GetDeviceType**() -> `DeviceType`
- **GetFocusedTextBox**() -> `TextBox`
- **GetGamepadConnected**(`gamepadNum: UserInputType`) -> `bool`
- **GetGamepadState**(`gamepadNum: UserInputType`) -> `Instances`
- **GetImageForKeyCode**(`keyCode: KeyCode`) -> `ContentId`
- **GetKeysPressed**() -> `Instances`
- **GetLastInputType**() -> `UserInputType`
- **GetMouseButtonsPressed**() -> `Instances`
- **GetMouseDelta**() -> `Vector2`
- **GetMouseLocation**() -> `Vector2`
- **GetNavigationGamepads**() -> `Array`
- **GetPasteText**() -> `string`
- **GetPlatform**() -> `Platform`
- **GetStringForKeyCode**(`keyCode: KeyCode`, `format: KeyCodeStringFormat = Default`) -> `string`
- **GetSupportedGamepadKeyCodes**(`gamepadNum: UserInputType`) -> `Array`
- **GetUserCFrame**(`type: UserCFrame`) -> `CFrame` [Deprecated]
- **IsGamepadButtonDown**(`gamepadNum: UserInputType`, `gamepadKeyCode: KeyCode`) -> `bool`
- **IsKeyDown**(`keyCode: KeyCode`) -> `bool`
- **IsMouseButtonPressed**(`mouseButton: UserInputType`) -> `bool`
- **IsNavigationGamepad**(`gamepadEnum: UserInputType`) -> `bool`
- **RecenterUserHeadCFrame**() -> `null`
- **SendAppUISizes**(`statusBarSize: Vector2`, `navBarSize: Vector2`, `bottomBarSize: Vector2`, `rightBarSize: Vector2`) -> `null`
- **SetNavigationGamepad**(`gamepadEnum: UserInputType`, `enabled: bool`) -> `null`

## Events

- **DeviceAccelerationChanged**(`acceleration: InputObject`)
- **DeviceGravityChanged**(`gravity: InputObject`)
- **DeviceRotationChanged**(`rotation: InputObject`, `cframe: CFrame`)
- **GamepadConnected**(`gamepadNum: UserInputType`)
- **GamepadDisconnected**(`gamepadNum: UserInputType`)
- **InputBegan**(`input: InputObject`, `gameProcessedEvent: bool`)
- **InputChanged**(`input: InputObject`, `gameProcessedEvent: bool`)
- **InputEnded**(`input: InputObject`, `gameProcessedEvent: bool`)
- **JumpRequest**()
- **LastInputTypeChanged**(`lastInputType: UserInputType`)
- **PointerAction**(`wheel: float`, `pan: Vector2`, `pinch: float`, `gameProcessedEvent: bool`)
- **StatusBarTapped**(`position: Vector2`)
- **TextBoxFocusReleased**(`textboxReleased: TextBox`)
- **TextBoxFocused**(`textboxFocused: TextBox`)
- **TouchDrag**(`dragDirection: SwipeDirection`, `numberOfTouches: int`, `gameProcessedEvent: bool`)
- **TouchEnded**(`touch: InputObject`, `gameProcessedEvent: bool`)
- **TouchLongPress**(`touchPositions: Array`, `state: UserInputState`, `gameProcessedEvent: bool`)
- **TouchMoved**(`touch: InputObject`, `gameProcessedEvent: bool`)
- **TouchPan**(`touchPositions: Array`, `totalTranslation: Vector2`, `velocity: Vector2`, `state: UserInputState`, `gameProcessedEvent: bool`)
- **TouchPinch**(`touchPositions: Array`, `scale: float`, `velocity: float`, `state: UserInputState`, `gameProcessedEvent: bool`)
- **TouchRotate**(`touchPositions: Array`, `rotation: float`, `velocity: float`, `state: UserInputState`, `gameProcessedEvent: bool`)
- **TouchStarted**(`touch: InputObject`, `gameProcessedEvent: bool`)
- **TouchSwipe**(`swipeDirection: SwipeDirection`, `numberOfTouches: int`, `gameProcessedEvent: bool`)
- **TouchTap**(`touchPositions: Array`, `gameProcessedEvent: bool`)
- **TouchTapInWorld**(`position: Vector2`, `processedByUI: bool`)
- **UserCFrameChanged**(`type: UserCFrame`, `value: CFrame`) [Deprecated]
- **WindowFocusReleased**()
- **WindowFocused**()
